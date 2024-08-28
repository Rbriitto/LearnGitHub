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


## Configure a ferramenta 
Configure informações de usuário para todos os repositórios locais
###### Referência: training.github.com
    
        $ git config --global user.name "[nome]"

*Configura o nome que voce quer ligado as suas transações  de commit.*

        $ git config --global user.email "[endereco-de-email]"

*Configura o email que você quer ligado as suas transações de commit*

        $ git config --global color.ui auto

*Configura o email que você quer ligado as suas transações de commit*

## Crie Repositórios 

        $ git init [nome-do-projeto]
*Cria um novo repositório local com um nome específico*

        $ git clone [url]
*Baixa um projeto e seu histórico de versão inteiro*

## Faça Mudanças 
Revise edições e crie uma transação de commit 

        $ git status

*Lista todos os arquivos novos ou modificados para serem commitados*

        $ git add [arquivo]
*Faz o snapshot de um arquivo na preparação para versionamento*

        $ git reset [arquivo]
*Deseleciona o arquivo, mas preserva seu conteúdo*

        $ git diff
*Mostra diferenças no arquivo que não foram realizadas* 

        $ git diff --staged
*Mostra a diferença entre arquivos selecionados e a suas últimas versões*

        $ git commit -m "[mensagem descritiva]"
*Grava o snapshot permanentemente do arquivo no histórico de versão*

## MUDANÇAS EM GRUPO
Nomeie uma série de commits e combine os esforços completos

        $ git branch
*Lista todos os branches locais no repositório atual*

        $ git branch [nome-do-branch]
*Cria um novo branch*

        $ git checkout [nome-do-branch]
*Muda para o branch específico e atualiza o diretório de trabalho*

        $ git merge [branch]

*Combina o histórico do branch específico com o branch atual*

        $ git branch -d [nome-do-branch]
*Exclui o branch específico*


## REFATORE NOMES DOS ARQUIVOS
Mude e remova os arquivos versionados

        $ git rm --cached [arquivo]
*Remove o arquivo do controle de versão mas preserva o arquivo localmente*

        $ git rm [arquivo]
*Remove o arquivo do diretório de trabalho e o seleciona para remoção*

        $ git mv [arquivo-original [arquivo-renomeado]
*Muda o nome do arquivo e o seleciona para o commit*


## SUPRIMA O RASTREAMENTO
Exclua arquivos e diretórios temporários

        *.log
        build/
        temp-*

*Um arquivo de texto chamado `.gitignore` suprime o versionamento acidental de arquivos e diretórios correspondentes aos padrões específicados*

        $ git ls-files --other --ignored --exclude-standard

*Lista todos os arquivos ignorados neste projeto*

## SALVE FRAGMENTOS
Arquive e restaure mudanças incompletas

        $ git stash
*Armazena temporariamente todos os arquivos rastreados modificados*

        $ git stash list
*Lista todos os conjuntos de alterações em stash*

        $ git stash pop
*Restaura os arquivos recentes em stash*

        $ git stash drop
*Descarta os conjuntos de alterações mais recentes em stash*

## REVISE HISTÓRICO
Navegue e inspecione a evolução dos arquivos do projeto

        $ git log
*Lista o histórico de versões para o branch atual*

        $ git log --follow [arquivo]
*Lista o histórico de versões para um arquivo, incluindo mudanças de nome*

        $ git diff [primerio-branch]...[segundo-branch]
*Mostra a diferença de conteúdo entre dois branches*

        $ git show [commit]
*Retorna mudanças de metadata e conteúdo para o commit especificado*

## DESFAÇA COMMITS
Apague enganos e crie um histórico substituto

        $ git reset [commit]
*Desfaz todos os commits depois de `[commit]`, preservando mudanças locais*

        $ git reset --hard [commit]
*Descarta todo histórico e mudanças para o commit especificado*


## SINCRONIZE MUDANÇAS
Registre um marcador de repositório e troque o histórico de versão

        $ git fetch [marcador]
*Baixe todo o histórico de um marcador de repositório*

        $ git merge [marcador]/[branch]
*Combina o marcador do branch no branch local*

        $ git push [alias] [branch]
*Envia todos os commits do branch local para o GitHub*

        $ git pull
*Baixa o histórico e incorpora as mudanças*









