# Passo a passo do projeto
 
## Criar projeto no VSCode

Criar um projeto. Sugestão aula-git.

## Instalar extensões no VSCode
 1. Aguardar um pouco
 2. Instalar depois para instalar quem tem mais de 10mi de downloads

## Criar/Inicializar umm projeto com git - git init

Rodar no terminal

```sh
git init
```

Perceba que o VSCode já destaca a integração com o GIT.


## Adicionando arquivos - git add
Os arquivos ainda sâo classificados como não rastreáveis(untraked)

Para eles comemeçarem a ser monitorados pelo git eles precisam ir para a área de staging. O comando:

```sh
git add *
```

O * é um coringa para adicionar tudo

## Persistir mudanças - git commit

Para persistir as mudanças, usamos o comando:
```sh
git commit -m 'feat-novo documento da aula'
```
## Criar um repositório no github

Uma vez criado o repositório no gitlab, ele vai sugerir diversos comandos que já executamos(git init, git add, git commit).

Vamos executar então o comando que vai parear e renomear nossa branch principal para main. Padrão atual github. Localmente estavamos com a branch principal chamada de master.

```sh
git branch -M main
```

O comando a seguir vai configurar o remote:
```sh
git remote add origin https://github.com/thiagok2/aula-git.git
```