
### Iniciando projeto git
Inicia um novo projeto como repositório git.
* Entre na pasta que deve ser um repositório


    
    git init


### Status

* Verificando status do repositório

    

    git status


### Lista 
* Arquivos


    git ls-files


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

* Criação de branch (-b)


    git checkout -b <nome_nova_branch> [<branch_a-ser-copiada>]



### Add
* Terminologia de status

   | STATUS  | DESCRIÇÃO|
   |:----------:|:-------------:|
   | Staged   |    Estado Monitoriado pelo git   |
   | Unstaged   |    Estado **NÃO** monitorado pelo git   |
   
   
 * Adicionando arquivos raiz (.)
    
    
    git add .
    

* Adicionando arquivo por caminho

    
    git add <caminho do repositório ou arquivo>



### Diff

Procurando diferença entre arquivos e repositórios

<br>
* Local / Arquivos


    git diff

<br>
* Repositórios


    git diff <branch.v1> <branch.v2>


### Log
Mostra informações dos historicos de commits realizados

    git log
    
### Whatchanged
Mostra informações dos historicos de commits realizados e arquivos que foram modificados

    git whatchanged (-p = detalhes)

### Remote

    git remote
    
* Enviando projeto para repositorio remoto
                
      git remote add origin https://github.com/<username>/<repository>.git
    

### Commit
      
      git commit -m 'Mensagem de commit' 
      

### Push


git push origin master