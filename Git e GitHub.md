# Git e GitHub <img src="https://img.shields.io/badge/Github-black?style=for-the-badge&logo=github&logoColor=white" > 


### O que é Git ? 
É Um Sistema de Controle de Versão Distribuído.<br> 
Gratuito e Open Source (Código Aberto).<br> 
Ramificações ( Branching) e fusões (merging) eficientes;<br> 
<b>Leve e Rápido</b>


https://git-scm.com/ <br> 
*Sempre ler a documentação e fazer um resumo*


### O que é GitHub ?
É Uma Plataforma De Hospedagem E Código Para Controle De Versão Com Git, E Colaboração.

##

### Configurando o Git

ctrl + L = Limpa o terminal 


git config --global user.name “rodrigo britto” (definindo o nome) <br>
git config --global user.email rodrigobritto.web@gmail.com (definindo o email)

git config user.name (retorna o nome) <br>
git config user.email (retorna o email)


Alterar a branch padrão:


git config user.name (retorna o nome) <br>
git config init.defaultBranch 
git config --global init.defaultBranch main (main é o nome padrão novo)			


## Autenticando Via Token

https://github.com/Rbriitto/hllo-world.git
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

## Protocolo SSH

https://docs.github.com/pt/authentication/connecting-to-github-with-ssh
.pub:  chave pública 

ssh-keygen -t ed25519 -C "rodrigobritto.web@gmail.com"<br>
passphrase: sorria<br>
cat : exibe o conteúdo do arquivo no bash


## Integrando o VSCODE com oo GITHUB

### O que é o GitIgnore ?


#### Utilizando O Git E Github

Versionamento de Código<br>
Sistemas de controle de versão<br>

### Controlam as versões de um arquivo ao longo do tempo

	Registra o histórico de atualizações de um arquivo
	Gerencia quais foram as alterações, a data, autor, etc;
	Organização, controle e segurança.

### Tipos de Sistemas de Controle de Versão 		
	
	Dentre os sistemas de Controle de Versão ( VCS), temos:

	VCS Centralizado (CVCS)
		Ex: CVS, Subversion.

	VCS Distribuído (DVCS)
		Ex: Git, Mercurial. 

<html>
<ul> <img src = "img/DVCS.png" width="1000"> </ul>
</html>


### Leia a documentação do projeto 

formato de link = [link](www.link.com).

Criar o clone na máquina para fazer as alterações e posteriormente estar implementando ela 


    1 - Escolha o Repositório que deseja utilizar 


|2 - Clique em Fork| <img src="img/fork.png">|
|--------------|-------------------------|
            
    3 - Vá nos seus repositórios e verifique se foi adicionado 
    4 - Copie o Link do GitHub 

<br>


## Clonando O Diretório.<br>
Dentro do Git Bash dar o comando: <b> $git clone “link-copiado-do-git-hub” </b>

Entrar na pasta <b>main</b> do projeto:  
<b>$ cd nome-da-pasta</b>

<b>$git remote -v </b>

Comando <b>$git remote -v </b> é usado para listar todos os repositórios remotos que estão configurados para o repositório local atual. O comando mostra os URLs associados a cada nome de repositório remoto, tanto para as operações de fetch (obter dados do remoto) quanto de push (enviar dados para o remoto).


<b>upstream</b> geralmente se refere ao repositório remoto original de onde um repositório foi clonado. Esse termo é usado especialmente quando você está contribuindo para um projeto que não é de sua autoria, mas para o qual você fez um fork.


<b>git remote add upstream</b> https://github.com/usuario-original/repositorio.git<br>
O comando <b>git pull</b> é usado para atualizar o repositório local com as mudanças do repositório remoto. Em resumo, ele faz duas coisas:

<b>git fetch</b>: Primeiro, ele busca (fetch) as atualizações do repositório remoto, trazendo todas as novas alterações e commits que não estão no repositório local.

<b>git merge</b>: Em seguida, ele mescla (merge) essas alterações da branch remota com a branch atual no repositório local.

O resultado é que a branch local é atualizada com as últimas mudanças feitas na branch correspondente no repositório remoto.

Em resumo:
<b>git pull </b> é uma combinação de <b>git fetch</b> e <b>git merge</b>, usada para trazer e integrar as mudanças do repositório remoto no seu repositório local.

<b> touch </b>: Ele é usado para criar arquivos vazios ou atualizar a data e hora de modificação de arquivos existentes.

#### Exemplos de Uso do <b> touch </b>:
Criar um novo arquivo vazio:

<b> touch </b> novo-arquivo.txt
Isso cria um arquivo vazio chamado novo-arquivo.txt no diretório atual.

Atualizar a data de modificação de um arquivo existente:

<b> touch arquivo-existente.txt</b> <br>
Isso não altera o conteúdo do arquivo, mas atualiza a data de modificação para a data e hora atuais.

Como o <b> touch </b> pode ser usado em conjunto com <b>*Git/GitHub:*</b><br>
Criar um arquivo antes de “comitar”: Se você deseja adicionar um novo arquivo ao seu repositório Git, pode usar <b> touch </b> para criá-lo e, em seguida, adicionar e “comitar” esse arquivo ao repositório.

* touch novo-arquivo.txt
* git add novo-arquivo.txt
* git commit -m "Adiciona novo arquivo vazio"
* git push origin main


#### Criar um README.md:
É comum usar <b> touch </b> para criar um arquivo README.md antes de escrever a documentação do projeto.

O <b> touch </b> é uma ferramenta útil no fluxo de trabalho, mas é independente do  <b>*Git ou GitHub*</b>. É usado para manipulação básica de arquivos no sistema de arquivos.


https://github.com/Rbriitto/dio-lab-open-source/blob/main/CONTRIBUTING.md


### Dicas e Materiais de Apoio


Encontre um projeto do seu interesse e adicione ao seu portfólio indicando a forma como contribui.
Participe da comunidade e desenvolvam juntos;
Conheça e respeite o padrão do projeto que for contribuir.
Bônus: Como editar arquivos pelo Github.

Ler a documentação e guia de contribuição 

### Configure a ferramenta 
Configure informações de usuário para todos os repositórios locais 
    
        $ git config --global user.name "[nome]"

*Configura o nome que voce quer ligado as suas transações  de commit.*

        $ git config --global user.email "[endereco-de-email]"

*Configura o email que você quer ligado as suas transações de commit*

        $ git config --global color.ui auto

*Configura o email que você quer ligado as suas transações de commit*
















