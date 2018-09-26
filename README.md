# devweb-app

## Como instalar
Se não tiver, instale o git e crie uma conta.

Então, pelo terminal vá até a pasta onde estará o projeto e coloque o comando:
```
git remote clone https://github.com/odair-silva/frameworkPET.git
git checkout -b frontend
git pull origin frontend
```
Isso irá baixar o projeto nessa pasta.
Recomendo esse site para comandos básicos de git: http://rogerdudler.github.io/git-guide/

Caso não tenha, baixe o nodejs 8.12 LTS: https://nodejs.org/en/

Depois de instalar o node, na pasta do projeto use o comando:
```
npm install
```
Esse comando deve instalar todas as dependências que eu usei até agora, essas dependências ficam no arquivo _package.json_ 


### Compilar e reloads usando o vuejs
```
npm run serve
```
Depois disso, vai aparecer um link com _localhost_ para abrir a página.

Digitando o comando:
```
vue ui
```
uma página com _dashboard_ vai estar disponível para gerenciar o projeto.
