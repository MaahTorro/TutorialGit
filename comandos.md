## Comandos principais do Git

### git init
```shell
git init
```
Inicia um novo repositorio git na pasta atual que se encontra o terminal

### git remote add
```shell
git remote add origin git@github.com:Maahtoro/at2tri.git
```
Adiciona um remote com o nome especificado com a url de origem especificada

Nesse caso estamos adicionando uma origem de nome “origin” que possui o servidor de origem git “github.com:Maahtoro/at2tri.git”

### git add
```shell
git add arquivo.js
```
caso queira adicionar todos os arquivos
```shell
git add .
```
Esse comando adiciona um ou varios arquivos para os arquivos para a staging da branch atual

### git branch
```shell
git branch nomeDaBranch
```
Esse comando cria uma nova branch com o nome especificado

Vale lembrar que ao criar uma branch ela usara SEMPRE como base a branch em que voce estava antes

### git checkout
```shell
git checkout nomeDaBranch
```
Esse comando faz com que o git va para a branch com o nome especificado

OBS: Se vc usar o seguinte comando:
```shell
git checkout -b nomeDaBranch
```
O git verifica primeiro se a branch existe, se nao ele cria, e apos isso fara o checkout, ou seja esse comando sao 2 em 1 caso a branch nao exista:
```shell
git branch nomeDaBranch
git checkout nomeDaBranch
```

### git fetch
```shell
git fetch origin
```
Esse comando faz um pull de todas as branchs de um remote especifico ou de todos caso vc passe --all no lugar do nome do remote (origin)

### git commit
```shell
git commit -m “mensagem resumindo as alteracoes”
```
Esse comando realiza um commit com a mensagem especificada dentro de aspas. (eh isso q o -m significa, m de message)

### git pull
```shell
git pull origin main
```
Esse comando realiza um pull das alteracoes do remote de nome “origin” e da branch “main” 

### git push
```shell
git push -u origin main
```
Esse comando realiza um push das alteracoes do remote de nome “origin” e da branch “main”, o -u serve para indicar q vc quer somente enviar as alteracoes desse remote e dessa branch

### git merge
```shell
git merge main
```
Esse comando realiza um merge da branch atual para a branch especificada