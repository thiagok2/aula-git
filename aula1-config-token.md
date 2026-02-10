# USAR O TOKEN / CRIAR TOKEN

0. No github

1. No ícone do seu usuário / clicar em settings / 

2. Na nova página, no menu lateral, Deveper Settings

3. No menu da esquerda, Personal Access Token

Fained Grained Token

4. ** Criar o token e guardar o número**

 
Com esse número vai fazer o comando

```sh
git remote set-url origin https://SEUTOKEN@github.com/SEUUSUARIO/SEUREPOSITORIO
```
 
```sh
git push -u origin main
```

5. Vamos alterar o nome do usuário - garantir que seja seu usuário/email configurado. Configurando local.

git config user.email "thiagok2@gmail.com"
git config user.name "thiagok2"

Obs.: Se a máquina for sua user o parâmetro --global
git config --globaluser.email "thiagok2@gmail.com"