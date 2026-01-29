# 🎵 Playlist Manager: Clean Code & Architecture

Este projeto foi desenvolvido como parte do meu processo de transição de carreira para o desenvolvimento de software. Trata-se de um sistema de gerenciamento de playlists via terminal (prompt), focado na aplicação prática de **Clean Code**, **Arquitetura de Software** e boas práticas com **Python**.

## 🧠 Conceitos de Clean Code Aprendidos

Durante o desenvolvimento, priorizei a escrita de um código que seja legível, testável e fácil de manter. Os principais pilares aplicados foram:

* **Responsabilidade Única (SRP):** Cada classe e método possui uma única tarefa clara, delegando para cada elemento somente uma única tarefa.
* **Commits Atômicos:** O histórico do Git foi construído como uma ferramenta de organização, onde cada commit representa uma pequena alteração lógica e independente.
* **Type Hinting:** Uso de anotações de tipo para tornar o código autodocumentado, facilitando a compreensão de quais dados são esperados e retornados.
* **Tratamento de Exceções:** Implementação de blocos `try/except` para gerenciar falhas de forma elegante e garantir que o sistema não quebre abruptamente.

## 🏗️ Arquitetura e Estrutura de Pastas (MVC + Constructor)

A maior entrega deste projeto é a sua organização estrutural. O sistema foi dividido seguindo o padrão **MVC**, mas com a adição de uma camada de **Constructor** para gerenciar as dependências:

* **Model:** Representação dos dados (entities) e ações de banco de dados, como busca e inserção (repositories).
* **View:** Responsável pela interação direta com o usuário (inputs e outputs).
* **Controller:** Onde reside a regra de negócio; processa as informações coletadas na View.
* **Constructor:** Camada que faz o "agrupamento" das responsabilidades, instanciando as classes e conectando View e Controller.

### 🔗 Correlação de Arquivos
Para manter a clareza e facilitar a manutenção, utilizei uma estratégia de nomes correlacionados. Arquivos que pertencem à mesma funcionalidade possuem nomes semelhantes em pastas diferentes, como:
- `song_register_view.py` (na pasta View)
- `song_register_controller.py` (na pasta Controller)
- `song_register_constructor.py` (na pasta Constructor)

Isso permite uma navegação intuitiva pelo projeto, onde é possível rastrear o fluxo de uma informação apenas pelo nome do arquivo.

## 🛠️ Tecnologias e Ambiente

* **Python 3**
* **Git** (Versionamento e fluxo profissional)
* **Ambiente Linux (Ubuntu)**
* **VS Code** (Configurações de produtividade e `settings.json` customizado)

---

### 🚀 Como executar o projeto

1. Clone o repositório.
2. No terminal, execute o ponto de entrada do sistema:
   ```bash
   python3 run.py