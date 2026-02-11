# Passo a passo do projeto
 
## Criar projeto no VSCode

Criar um projeto: Sugestão aula-git. Criar pasta e abrir pasta no VSCode.

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
Criar arquivo, como por exemplo aula1.md. 
Escrever um texto dentro do aula1.md.

Os arquivos ainda sâo classificados como não rastreáveis(untraked)

Para eles comemeçarem a ser monitorados pelo git eles precisam ir para a área de staging. O comando:

```sh
git add *
```

O * é um coringa para adicionar tudo

## Persistir mudanças LOCALMENTE - git commit

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
git remote add origin https://github.com/SEUUSUARIO/SEUREPOSITORIO.git
```

Feito isso, para enviar definitivamente seus arquivos para o github execute:

```sh
git push origin main
```

# Possíveis problemas:

## Necessidade de definir user.name e user.email 
Boa prática é definir o usuário e email do seu usuário localmente. As vezes o git pode apontar erro ou passar a informação de outro usuário ao github.

Consultando configuração atual
```sh
git config user.email
git config user.name
```

Vamos alterar o nome do usuário - garantir que seja seu usuário/email configurado. Configurando local.
```sh
git config --local user.email "thiagok2@gmail.com"
git config --local user.name "thiagok2"
```

Obs.: Se a máquina for sua user o parâmetro --global
```sh
git config --global user.email "thiagok2@gmail.com"
git config --global user.email "thiagok2"
```

### Configurar usuário e token

Ir para o conteúdo da aula1-config-token.

### Problema de branchs divergentes e histórias não relacionadas

**Repositórios com trabalhos desalinhados**

Há trabalhos/arquivos/modificações no repositório remoto e não estão localmente.
Para trazer o trabalho(arquivos, mudanças) do remoto, execute:

```sh
git pull origin main
```

Obs.: Para fazer um pull é necessário que nâo haja código a ser commitado. Logo, será necessário executar:

```sh
git add *
git commit -m 'finalizando tarefa'
```

E então fazer push:
```sh
git push origin main
```

#### Caso receba a mensagem de branchs divergentes, vamos fazer o rebase

Ainda assim, podem haver erros FATAIS. Que podem ser devido a um desalinhamento/divergência das branchs, histórias não relacionadas.

Como resolver:
```sh
git config pull.rebase true
```
