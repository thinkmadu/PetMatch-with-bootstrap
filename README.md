# Sistema de adoção de pets - PETMATCH (ver. 2)
Esse projeto é uma remodelação do projeto PetMatch (sistema desenvolvido para a disciplina de Gerência de Projetos) e será adaptado para atender aos critérios da disciplina de Programação Web.

## Ferramentas utilizadas no projeto
- MySql 8.x.x ou superior.
- Python 3.11 ou superior.
- BootStrap

## Documentação
- [Documento de visão](

## Passo a passo para execução
### Instalando pacotes necessários
- Execute no terminal o comando `pip install -r requirements.txt`

### Configurando o banco de dados pré-existente
- O projeto, por padrão, já possui um banco de dados alimentado com pets de exemplo. Para utilizá-lo, siga os passos abaixo:
1. No MySQL Workbench, selecionar uma conexão.
![img.png](img.png)
2. Vá em *Server* -> *Data Import* -> navegue até a pasta *PetmatchExport* -> *Import Progress* -> *Start Import*
![img_1.png](img_1.png) ![img_2.png](img_2.png)
3. Agora com o banco de dados importado, é necessário configurar as credenciais de acesso ao banco de dados no arquivo `app.py` na linha 22. Siga o padrão: `app.config['SQLALCHEMY_DATABASE_URI'] = 'mysql+pymysql://<nome_do_user_mysql>:<senha_do_user>@localhost/PetMatch'`
4. Execute o arquivo PetMatch.py, no terminal irá aparecer a url do servidor local para acessar o sistema.

## Credenciais
Caso vocẽ use o banco de dados já alimentado, já existem credenciais de acesso para os usuários, ongs e administradores.
| Tipo de usuário| Email                  | Senha|
|----------------|------------------------|------|
|Admin           |admin1@gmail.com        | 77   |
|Admin           |admin2@gmail.com        | 88   |
|Admin           |admin3@gmail.com        | 77   |
|Admin           |admin4@gmail.com        | 88   |
|Ong             |a4ong@gmail.com         | 11   |
|Ong             |animalderuacg@gmail.com | 11   |
|Usuário normal  |doxino2895@aqqor.com    | 00   |
|Usuário normal  |melobos118@chainds.com  | 11   |
|Usuário normal  |sohew17721@confmin.com  | 22   |

