## Instalando o Git

Para isso, escolha seu sistema operacional na página de [Downloads]() do projeto e siga as instruções de instalação do programa.

<br>

**Windows**<br>
Para instalarmos o git, basta fazermos o download no link acima e seguirmos as instruções de instalação do próprio instalador.

<br>

**Linux**<br>
Para instalarmos o Git no Linux utilizaremos apt-get.

Abra o terminal do Linux e digite o comando abaixo:

* Ububtu
    ```bash
    sudo apt-get install git
    ```
* Fedora
    ```bash
    sudo dnf -y install git
    ```
Agora é só colocar sua senha e aguardar a instalação.    

<br>

**MacOS**<br>

Para instalarmos o Git no MacOS utilizaremos o gerenciador de downloads Brew.

Caso você não tenha o Brew instalado, rode o comando abaixo:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Aguarde a instalação do Brew e prossiga executando o comando abaixo:

    brew install git


<br>


### Configuração<br>

Verifique a versão do git que foi instalada executando o seguinte comando:
 
    git --version

Para evitar erros de commit, é uma boa idéia configurar seu usuário para git (use a opção **–global** para especificar as configurações globais / todo computador). 
            
    git config --global user.name "sampleuser"
    git config --global user.email "sampleuser@example.com"
   

Você pode verificar as alterações de configuração visualizando o .gitconfig:

    git config --list

Isso deve produzir uma saída semelhante à seguinte:

```bash
[root@host ~]# git config --list
user.name=sampleuser
user.email=sampleuser@example.com
```     
