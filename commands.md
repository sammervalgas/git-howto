
### Iniciando projeto git
Inicia um novo projeto como repositório git.
* Entre na pasta que deve ser um repositório


    git init


### Status

* Verificando status do repositório

    
    git status


### Lista



### Clonando o projeto

    git clone https://github.com/<username>/<repositorio>.git

### Tag
* Quantas versões exitem do projeto
    
    
    git tag
    
    
### Checkout
Trocando de repositórios:

<br>
* Local
    
    git checkout <Nome da branch ou tag>

<br>
* Remoto
    
    git checkout origin <Nome da branch>

<br>

### Add
* Terminologia de status

   | STATUS  | DESCRIÇÃO|
   |:----------:|:-------------:|
   | Staged   |    Estado Monitoriado pelo git   |
   | Unstaged   |    Estado **NÃO** monitorado pelo git   |
   
   
 * Adicionando arquivos raiz (.)
    
    
    git add .
    

* Adicionando arquivo por caminho

    
    git add <caminho do repositório>



### Diff

Procurando diferença entre arquivos e repositórios

<br>
* Local / Arquivos


    git diff

<br>
* Repositórios


    git diff <branch.v1> <branch.v2>
