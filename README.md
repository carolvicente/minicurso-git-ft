# Minicurso de Git - Semana da Tecnologia em Foco 2018


Minicurso Git - 2:30 hrs

Quem somos nós
O que é o Git? Diferenças entre outros sistema de Versionamento


# Vamos começar!

### Configurações Iniciais

* Cadastro no Github
* Install Git no Desktop   https://git-scm.com/downloads
* Configuração do Git : 
	git config --[option] user.name "seu_nome" . 
	git config --[option] user.email "seu email" . 

	option : global ou local . 

### Criando um Projeto no Git

* Criação Repositório 
* Adicionar Colaboradores 
* git clone 
 
 
### Git Status 

* Teoria:

Untracked :
Arquivo não mapeado pelo Git.  
O Git está vendo um arquivo que não existia na última captura (commit);  
Git não vai incluí-lo nas suas capturas de commit até que você o diga explicitamente que assim o faça.  

Unmodified : 
Nenhum arquivo foi modificado na branch atual.  

Modified : 
Há arquivos modificados na branch atual.  

Staged : 
O Arquivo foi selecionado para o próximo commit.  

* Comando git status . 

### Criação de Branches . 

* Teoria: 
O Git permite criar uma linha independente de desenvolvimento no seu projeto. Isto permite alterações em partes específicas do software sem comprometer o restante do projeto. Essas linhas independentes são chamadas de branches. 

* Criar nova branch :
git branch testing   
Mudar de branch   
git checkout "nome_da_branch" . 

* Tudo em um : ou git checkout -b "nome_da_nova_branch" . 

### Criação de um Commit

git add * , git add, git commit, git commit amend . 
git push . 

### Fazendo um merge

git checkout master  
git merge "nome_da_sua_branch" . 

### Dinâmicas

[Dinâmica - 1]
Cada um cria uma branch sua, e com arquivos diferentes.  
Performa as ações de commit e de merge na master.  

[Dinâmica - 2]
Cada um cria uma branch sua, e com arquivos diferentes.  
O Colega 1 pegas as alterações do Colega 2.  
Performa as ações de commit e de merge na master.  

[Dinâmica - 3]
Cada um cria uma branch sua, e com arquivos diferentes.  
O Colega 1 pegas as alterações do Colega 2, e faz modificações nesse arquivo.  
Colega 2 atualiza seu repositório, faz o merge da Branch do Colega 1, vê que tem conflitos, resolve os conflitos.  
Colega 2 performa as ações de commit e de merge na master. 
