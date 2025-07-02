# Imersão DevOps - Alura Google Cloud: API de Gestão Educacional

Este projeto apresenta uma API RESTful desenvolvida com FastAPI para o gerenciamento de alunos, cursos e matrículas em uma instituição de ensino.

## Pré-requisitos

Para executar esta aplicação, certifique-se de ter os seguintes softwares instalados:

- [Python 3.10 ou superior instalado](https://www.python.org/downloads/)
- [Git](https://git-scm.com/downloads)
- [Docker](https://www.docker.com/get-started/)

## Configuração e Execução

1. **Download do repositório:**
   [Baixe o projeto](https://github.com/MaduAraujo/API-Gestao-Escolar/archive/refs/heads/main.zip)

2.  **Criação do Ambiente Virtual:**<br>
    Navegue até o diretório raiz do projeto e crie um ambiente virtual Python:

    ```sh
    python3 -m venv ./venv
    ```
    
3.  **Instalação de Dependências:**<br>
    Com o ambiente virtual ativado, instale as bibliotecas necessárias listadas em `requirements.txt`:

    ```sh
    pip install -r requirements.txt
    ```

4.  **Ativação do Ambiente Virtual:**<br>
    Ative o ambiente virtual recém-criado:

      * **Linux/macOS:**
        ```sh
        source venv/bin/activate
        ```
      * **Windows:**
        Abra o terminal como administrador e execute os seguintes comandos:
        ```powershell
        Set-ExecutionPolicy RemoteSigned
        venv\Scripts\activate
        ```

5. **Execute a aplicação:**
   ```sh
   uvicorn app:app --reload
   ```

6. **Acesse a documentação interativa:**

   Abra o navegador e acesse:  
   [http://localhost:8000/docs](http://localhost:8000/docs)

   Aqui você pode testar todos os endpoints da API de forma interativa.

## Estrutura do Projeto

```markdown
├── .dockerignore
├── .gitattributes
├── .gitignore
├── .pycache/
├── Dockerfile
├── app.py
├── database.py
├── docker-compose.yml
├── escola.db
├── models.py
├── readme.md
├── requirements.txt
├── routers/
│   └── **init**.py  (Assumindo que este arquivo esteja dentro, mesmo que não mostrado explicitamente)
└── schemas.py
└── venv/
```

- `app.py`: Arquivo principal da aplicação FastAPI.
- `models.py`: Modelos do banco de dados (SQLAlchemy).
- `schemas.py`: Schemas de validação (Pydantic).
- `database.py`: Configuração do banco de dados SQLite.
- `routers/`: Diretório com os arquivos de rotas (alunos, cursos, matrículas).
- `requirements.txt`: Lista de dependências do projeto.

---

**Observações:**

  * O banco de dados SQLite (`escola.db`) será automaticamente criado na primeira execução da aplicação, caso não exista.
  * Para redefinir o banco de dados e apagar todos os dados existentes, basta excluir o arquivo `escola.db`.

-----

## API Interativa

<p align="center">
  <img src="https://github.com/user-attachments/assets/a161fb7f-1ec7-4b87-8ed4-6f87378dcbff" width="800">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/0ae003b1-af94-4c06-bf09-1ef45d68fea3" width="800">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/468b29c7-f44d-4f55-84b7-599591bb2a9c" width="800">
</p>
