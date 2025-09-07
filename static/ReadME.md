# PCP-Flow: Gestão de Projetos com Gráfico de Gantt

> Aplicação web local para gestão de projetos e tarefas das áreas de PCP e Suprimentos, com foco na geração de gráficos de Gantt dinâmicos e visualmente personalizáveis para manter a identidade visual da empresa.

![PCP-Flow Screenshot](Gantt%20Analyst%20Copilot.png)  

---

## 📋 Índice

- [Funcionalidades Principais](#-funcionalidades-principais)
- [Tecnologias Utilizadas](#️-tecnologias-utilizadas)
- [Começando](#-começando)
  - [Pré-requisitos](#pré-requisitos)
  - [Instalação](#instalação)
- [Como Executar](#-como-executar)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Roadmap (Melhorias Futuras)](#-roadmap-melhorias-futuras)
- [Licença](#-licença)

---

## ✨ Funcionalidades Principais

- **Gestão de Tarefas (CRUD):** Crie, leia, atualize e delete tarefas de forma simples e intuitiva.
- **Gráfico de Gantt Dinâmico:** O cronograma é gerado e atualizado automaticamente a partir da lista de tarefas.
- **Persistência de Dados:** As tarefas são salvas em um banco de dados local (SQLite), garantindo que os dados não sejam perdidos.
- **Interface Web Local:** Rode a aplicação diretamente no seu navegador, sem depender de serviços externos.
- **Alta Personalização Visual:** O gráfico de Gantt é estilizado para mimetizar a aparência de relatórios do Excel, mantendo a padronização visual.
- **Localização em Português:** Toda a interface, incluindo eixos do gráfico e textos de hover, está em PT-BR.

---

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando as seguintes tecnologias:

- **Backend:**
  - [Python 3](https://www.python.org/)
  - [Flask](https://flask.palletsprojects.com/): Micro-framework web para a criação da API e da lógica do servidor.
  - [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/): ORM para interação com o banco de dados.
- **Banco de Dados:**
  - [SQLite](https://www.sqlite.org/index.html): Banco de dados relacional embarcado, ideal para aplicações locais.
- **Análise e Gráficos:**
  - [Pandas](https://pandas.pydata.org/): Utilizado para a estruturação dos dados antes da plotagem.
  - [Plotly](https://plotly.com/python/): Biblioteca para a geração de gráficos interativos e de alta qualidade.
- **Frontend:**
  - HTML5
  - CSS3

---

## 🚀 Começando

Siga as instruções abaixo para obter uma cópia do projeto e executá-lo na sua máquina local.

### Pré-requisitos

- **Python 3.8+** instalado. Você pode verificar sua versão com `python --version`.
- **pip** (gerenciador de pacotes do Python) instalado.

### Instalação

1.  **Clone o repositório ou baixe os arquivos** para um diretório de sua preferência.

2.  **Crie um ambiente virtual (recomendado):**
    Abra o terminal no diretório do projeto e execute:
    ```bash
    # Para Windows
    python -m venv venv

    # Para macOS/Linux
    python3 -m venv venv
    ```

3.  **Ative o ambiente virtual:**
    ```bash
    # Para Windows
    .\venv\Scripts\activate

    # Para macOS/Linux
    source venv/bin/activate
    ```

4.  **Instale as dependências:**
    Crie um arquivo chamado `requirements.txt` na raiz do projeto com o seguinte conteúdo:
    ```
    Flask
    Flask-SQLAlchemy
    pandas
    plotly
    ```
    Em seguida, instale todas as dependências de uma vez com o comando:
    ```bash
    pip install -r requirements.txt
    ```

---

## 🏃 Como Executar

Com o ambiente virtual ativado e as dependências instaladas, basta executar o seguinte comando no terminal:

```bash
python app.py