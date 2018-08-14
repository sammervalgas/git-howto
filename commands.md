
### Iniciando projeto git
Inicia um novo projeto como repositório git.
* Entre na pasta que deve ser um repositório
```bash
git init
```

### Status
* Verificando status do repositório
```bash
git status
```
### Lista 

    git ls-files


### Clonando o projeto
```bash
git clone https://github.com/<username>/<repositorio>.git
```


### Tag
* Quantas versões exitem do projeto
```bash
git tag
```
    
### Checkout
Trocando de repositórios:

<br>
* Local
    
    git checkout <Nome da branch ou tag>

<br>
* Remoto
    
    git checkout origin <Nome da branch>

* Criação de branch (-b)
```bash
git checkout -b <nome_nova_branch> [<branch_a-ser-copiada>]
```
### Add
* Terminologia de status

   | STATUS  | DESCRIÇÃO|
   |:----------:|:-------------:|
   | Staged   |    Estado Monitoriado pelo git   |
   | Unstaged   |    Estado **NÃO** monitorado pelo git   |
   
   
 * Adicionando arquivos raiz (.)
```bash
git add 
```
* Adicionando arquivo por caminho

```bash
git add <caminho do repositório ou arquivo>
```
    



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
* Mostra informações dos historicos de commits realizados e arquivos que foram modificados
```bash
git whatchanged (-p = detalhes)
```


### Remote

    git remote
    
* Enviando projeto para repositorio remoto
```bash
git remote add origin https://github.com/<username>/<repository>.git
```
                
    

### Commit
```bash
git commit -m 'Mensagem de commit' 
```
      

### Push

```bash
git push origin <nome_da_branch>
```

