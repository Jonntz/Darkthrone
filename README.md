# :spades: Darkthrone
## :computer: Projeto Interdisciplinar do curso de Análise e desenvolvimento de sistemas da Cruzeiro do Sul.
--------------

### Instalação e configuração

1. Primeiro de tudo, o python deve ser instalado globalmente:
   
   - **No linux**
     Provavelmente ele já vem instalado, mas caso não tenha instalado, basta rodar o seguinte comando:
     <br><br>
      `sudo apt-get install python3`
      <br><br>
   - **No windows**
     Basta acessar [este link]([https://www.python.org/downloads/windows/]), baixar a **última versão** e seguir os passos do instalador.
<br><br>

2. Após instalar o python, é necessário instalar um gerenciador de pacote. Como estamos trabalhando com python, é recomendando utilizar o PIP:
   - **No Linux**:
     Basta executar o comando no terminal:
     <br><br>
     `sudo apt-get install python-pip.`
    <br><br>

   - **No Windows**
     Abra o cmd como administrador e digite o seguinte comando:
     <br><br>
     `py -m ensurepip --upgrade`
     <br><br>

3. Instalando o postgres:
   - **No Linux**
      Execute o seguinte comando no terminal: 
      <br><br>
      `sudo apt update`<br>
      `sudo apt install postgresql postgresql-contrib`
      <br><br>
      Depois, instale o ambiente gŕafico, para gerenciamento do banco:
      <br><br>
      `sudo apt-get install pgadmin3`
      <br><br>


   - **No windows**
      No Windows, basta acessar o site do postgres [neste link](https://www.postgresql.org/download/windows/), baixar a versão mais recente e seguir os passos no instalador.
   

4. Com o Python e o PIP instalados, podemos montar nosso ambiente. Vamos começar instalando um ambiente virtual:
   `pip install virtualenv`

   - Em seguida basta clonar o projeto: `git clone https://github.com/Jonntz/Darkthrone`
   - Entre na pasta do projeto: `cd darkthrone`
   - Crie um ambiente virtual: `virtualenv env` **O nome do ambiente deve sempre ser 'env'**
   - Ative o ambiente virtual com o seguinte comando: `source env/bin/activate`
   - Instale todas as dependencias: `pip3 install -r requirements.txt;`
   - Faça as migrations para o banco de dados: 
    <br><br>
    `python manage.py makemigrations` <br>
    `python manage.py migrate;`
    <br><br>
   - Inicie a aplicação: `python manage.py runserver`
   

