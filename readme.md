# Imersão DevOps - Alura Google Cloud

Este projeto é uma API desenvolvida com FastAPI para gerenciar alunos, cursos e matrículas em uma instituição de ensino.

## Pré-requisitos

- [Python 3.10 ou superior instalado](https://www.python.org/downloads/)
- [Git](https://git-scm.com/downloads)
- [Docker](https://www.docker.com/get-started/)

## Passos para subir o projeto

1. **Faça o download do repositório:**
   [Clique aqui para realizar o download](https://github.com/MaduAraujo/API-Gestao-Escolar/archive/refs/heads/main.zip)

2. **Crie um ambiente virtual:**
   ```sh
   python3 -m venv ./venv
   ```

3. **Ative o ambiente virtual:**
   - No Linux/Mac:
     ```sh
     source venv/bin/activate
     ```
   - No Windows, abra um terminal no modo administrador e execute o comando:
   ```sh
   Set-ExecutionPolicy RemoteSigned
   ```
   
     ```sh
     venv\Scripts\activate
     ```

4. **Instale as dependências:**
   ```sh
   pip install -r requirements.txt
   ```

5. **Execute a aplicação:**
   ```sh
   uvicorn app:app --reload
   ```

6. **Acesse a documentação interativa:**

   Abra o navegador e acesse:  
   [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

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

