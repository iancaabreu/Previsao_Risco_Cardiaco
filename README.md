## Meu projeto 

Esse é o meu projeto 

### Instalação e Configuração

    1. Clone o repositório:

    ```bash
    git clone https://github.com/lvgalvao/dataprojectstarterkit.git
    cd dataprojectstarterkit
    ```

    2. Configure a versão correta do Python com `pyenv`:

    ```bash
    pyenv install 3.11.5
    pyenv local 3.11.5
    ```

    3. Instale as dependências do projeto:

    ```bash
    python -m venv .venv
    # O padrao é utilizar .venv
    source .venv/bin/activate
    # Usuários Linux e mac
    .venv\Scripts\Activate
    # Usuários Windows
    pip install -r requirements.txt  
    ```
Kit inicial de projeto de dados
Sobre o Projeto
Este repositório é uma parte integrante do workshop "Como estruturar um projeto de dados do Zero". O objetivo aqui é fornecer uma base e uma estrutura padronizada para iniciar projetos de engenharia, 
ciência e análise de dados. O foco principal é em boas práticas, automação, testes e documentação. Tera um novo no dia 29/01

Objetivos do Workshop:
Entender a estrutura padrão de projetos : Isso inclui a organização de diretórios, como o código-fonte, testes, documentos, entre outros.

Estruturas padrões em projetos de dados : Vamos refatorar o projeto utilizando classes, módulos e boas práticas em um ETL.

Familiarizar-se com ferramentas de desenvolvimento : Abordaremos o uso de ambientes virtuais e discutiremos ferramentas como PIP, CONDA e POETRY.

Testes com Pytest : Garante que seu código funcione como esperado, criando testes unitários e de integração.

Versionamento com Git e GitHub : Aprenda a versionar seu projeto e usar o GitHub para colaboração e publicação.

Documentação com MKDocs : Você vai aprender a documentar seu projeto com MKDocs e publicar suas documentos no GitHub Pages

Automatização e CI/CD : Configure rotinas de integração e entrega contínua para manter a qualidade do projeto.

Começando
Pré-requisitos
VSCode : É o editor de código que usaremos no workshop. Instruções de instalação do VSCode aqui .

Git e GitHub :

Você deve ter o Git instalado em sua máquina. Instruções de instalação do Git aqui .
Você também deve ter uma conta no GitHub. [Instruções de criação de conta no GitHub aqui] ( https://docs.github.com/pt/get-started/onboarding/getting-started-with-your-github-account ).
Se você for usuário Windows, recomendo esse vídeo: Youtube .
Tutorial de Git e Github básico Ebook .
Se você já é usuário Git, recomendo o vídeo do Akita: Youtube .
Pyenv : É usado para gerenciar versões do Python. Instruções de instalação do Pyenv aqui . Vamos usar nesse projeto o Python 3.11.3. Para usuários do Windows, é recomendado assistirem esse tutorial do Youtube .

Poesia : Este projeto utiliza Poesia para gerenciamento de dependências. Instruções de instalação do Poetry aqui . Se você é usuário Windows, recomendo assistir esse vídeo: Youtube . Que instala o Python, Poetry e VSCode. Mas um comando simples PIP INSTALL POETRY já resolve.

Sugestão de leituras. Ebook 1 - Testes Ebook 2 - Github Actions Ebook 3 - Na minha máquina funciona

Instalação e Configuração
Clone o repositório:
git clone https://github.com/lvgalvao/dataprojectstarterkit.git
cd dataprojectstarterkit
Configure a versão correta do Python com pyenv:
pyenv install 3.11.5
pyenv local 3.11.5
Configure poesia para Python versão 3.11.5 e ativo o ambiente virtual:
poetry env use 3.11.5
poetry shell
Instale as dependências do projeto:
poetry install
Execute os testes para garantir que tudo esteja funcionando conforme o esperado:
task test
Execute o comando para ver a documentação do projeto:
task doc
Execute o comando de execução do pipeline para realizar um ETL:
task run
Verifique na pasta de dados/saída se o arquivo foi gerado corretamente.
Contato
Para dúvidas, sugestões ou feedbacks:

Luciano Filho - lvgalvaofilho@gmail.com
