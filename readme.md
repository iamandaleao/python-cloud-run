# API de Gestão Escolar – Imersão Cloud & DevOps (Alura + Google Cloud)

Este projeto foi desenvolvido durante a **Imersão Cloud & DevOps**, promovida pela [Alura](https://www.alura.com.br) em parceria com o Google Cloud. A aplicação é uma **API em Python com FastAPI** para gerenciar alunos, cursos e matrículas.

## Funcionalidades

- Cadastro de alunos
- Cadastro de cursos
- Matrícula de alunos em cursos
- Documentação interativa com Swagger UI

## Acesse a API Online

A API está publicada no **Google Cloud Run** e pode ser testada diretamente no navegador:

[Documentação Interativa (Swagger UI)](https://api-747351593414.southamerica-east1.run.app/docs)

## Tecnologias e Ferramentas

- Python 3.10+
- FastAPI
- Docker e Docker Compose
- GitLab CI/CD
- Google Cloud Run
- SQLite (banco de dados local)
- Gemini Code Assist (para apoio com IA)
  
## Pré-requisitos

- [Python 3.10 ou superior instalado](https://www.python.org/downloads/)
- [Git](https://git-scm.com/downloads)
- [Docker](https://www.docker.com/get-started/)

## Passos para subir o projeto

1. **Faça o download do repositório:**
   [Clique aqui para realizar o download](https://github.com/iamandaleao/python-cloud-run/archive/refs/heads/main.zip)


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

---

## Estrutura do Projeto

- `app.py`: Arquivo principal da aplicação FastAPI.
- `models.py`: Modelos do banco de dados (SQLAlchemy).
- `schemas.py`: Schemas de validação (Pydantic).
- `database.py`: Configuração do banco de dados SQLite.
- `routers/`: Diretório com os arquivos de rotas (alunos, cursos, matrículas).
- `requirements.txt`: Lista de dependências do projeto.
-  `Dockerfile`: Imagem da aplicação.

---

- O banco de dados SQLite será criado automaticamente como `escola.db` na primeira execução.
- Para reiniciar o banco, basta apagar o arquivo `escola.db` (isso apagará todos os dados).

---
## Aprendizados na Imersão

- Criar e rodar contêineres com Docker  
- Resolver o “na minha máquina funciona” com ambiente isolado  
- Implementar CI/CD com GitLab  
- Automatizar build, testes e deploy  
- Fazer deploy real com Google Cloud Run  
- Usar IA (Gemini Code Assist) para apoio no desenvolvimento  

---

✨ Feito com dedicação por [Amanda Leão](https://github.com/iamandaleao) durante a Imersão Cloud & DevOps – uma jornada de aprendizado sobre Docker, CI/CD, deploy na nuvem e o poder da automação no desenvolvimento.


