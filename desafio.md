1. Criar fork do projeto no gitlab
ícone novo fork
https://github.com/thiagok2/aula-git/

2. Clonar o projeto localmente
clonar o seu projeto

No VSCode, em uma nova pasta, no terminal:
```sh
git clone https://github.com/seuusuario/seurepositorio.git
```

* Atenção ao clonar, no VSCode entrar na pasta do projeto clonado.

3. Criar uma branch
```sh
git checkout -b feat-customizacao
```
4. Trabalhar nela, sou seja adicionar arquivos e fazer commit;
```sh
git add *
git commit -m 'novos arquivos que trabalhei'
```

5. Fazer push da sua branch nova
```sh
git push origin feat-customizacao
```

6. Fazer merge na main com o código da sua branch
```sh
git checkout main
```

```sh
git merge feat-customizacao
```

```sh
git push origin main
```