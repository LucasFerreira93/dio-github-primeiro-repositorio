# Git e GitHub - Instalação, Configuração e Primeiros Passos

---------



## O que é o Git?

O [Git](https://www.treinaweb.com.br/blog/tag/git/) é um sistema de controle de versão distribuído, utilizado principalmente no desenvolvimento de software e, assim como diz em sua página inicial, tanto em projetos pequenos ou de grande porte. Gratuito e open source, foi desenvolvido por Linus Torvalds para o desenvolvimento do Kernel Linux (Código aberto para sistemas operacionais tipo Unix). Seu lançamento foi em 2005 e atualmente se encontra na versão 2.21.0 (24/02/2019).



## O que é o GitHub?

O [GitHub](https://github.com/) é a ferramenta que nos provê acesso ao Git para armazenarmos nossos códigos com todo poder do versionamento que o Git oferece.



## Como instalar

O primeiro passo para instalação do Git em sua máquina, é acessar o seu site para realizar o [download do Git](https://git-scm.com/).

Em seu site você encontra toda documentação, comunidade, download (para diferentes sistemas operacionais - Windows, Mac e Linux), empresas e projetos que utilizam o Git (Google, Facebook, Twitter, Netflix, entre outras) e muito mais



## Primeira Configuração

Configurar nossa conta para trabalhar com o Git, e isto é feito pelo comando **git config**, onde podemos informar nosso nome e E-mail.

Como estas configurações são globais, também devemos adicionar a opção --global ao comando, seguida dos valores entre aspas.

```
git config --global user.name "Priscila Ferreira"
git config --global user.email "seuemail@gmail.com"
```

Executando estes dois comandos, temos nosso nome e E-mail armazenados e a cada alteração que fizermos eles serão automaticamente adicionados.



## Iniciando um Repositório

Para começar a brincar com o Git/GitHub, vamos criar uma pasta em um local seguro. 

```
C:\Workspace
```

Isto fará a criação de uma nova pasta chamada **Workspace** . Logo apos feito isso vamos criar um novo arquivo chamado de **README.md** na raiz.

Por padrão, todo repositório no GitHub tenta buscar um arquivo README.md na raiz do projeto para exibi-lo na página inicial do repositório.

Os arquivos ".md" são no formato MarkDown, que é uma espécie de linguagem de marcação, assim como o HTML.



## Principais comandos

- Inicializar um diretório

Para inicializar um diretório utilizaremos o comando `git init`. Com ele é possível a criação de um diretório vazio (basicamente um diretório .git) ou a reinicialização de um diretório já existente.

- Clonar um repositório

​	Para copiar um diretório já existente, por exemplo, de um projeto que você queira contribuir, 	utilizaremos o comando `git clone`. Este comando irá criar uma cópia idêntica do projeto no seu computador para que seja feita alguma alteração em seus arquivos.

- Adicionar arquivos

  Para adicionar arquivos que serão, posteriormente, versionados pelo git, utilizamos o comando `git add`. Este comando irá adicionar um ou mais arquivos ao controle de versionamento do git, fazendo com que todas as alterações deste arquivo sejam monitoradas posteriormente. Todos os arquivos adicionados pelo `git add` são armazenados no INDEX, uma área onde todo o controle de versionamento acontece. Vale lembrar que o comando `git add` não está adicionando um novo arquivo ao repositório, ele só indica quais arquivos serão utilizados na nova versão do projeto.

- Commitar mudanças

Após determinar quais arquivos farão parte da nova versão de um projeto, utilizamos o comando `git commit` para criar um comentário que identifica essas novas alterações. Vale lembrar que o comando `git commit` também gera um número automático para identificar, de forma única, cada alteração no projeto.

- Enviar mudanças para o servidor

Depois de gerar um identificador para as alterações com o comando `git commit`, utilizamos o comando `git push` para enviar as alterações para o servidor git configurado em nosso repositório. Basicamente, é com este comando que fazemos o “upload” das alterações.

- Obter mudanças do servidor

Além de enviar alterações para o servidor, podemos capturar alterações que estejam salvas no servidor e não localmente. Para isso, utilizamos o comando `git pull`. Este comando é muito útil quando estamos desenvolvendo um projeto em equipe e precisamos obter as alterações feitas por outro membro do time.

- Obter status

Para obter o status das alterações feitas nos arquivos do repositório, utilizamos o comando `git status`. Este comando irá retornar a lista de arquivos que foram modificados e que podem ser enviados para o servidor.
