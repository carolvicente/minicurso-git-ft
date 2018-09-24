# Minicurso de Git - Semana da Tecnologia em Foco 2018


Duração: 2:30 hrs 

* Vamos nos apresentar :) 

* O que é o Git? 

Git é um sistema de controle de versão de arquivos. Através deles podemos desenvolver projetos na qual diversas pessoas podem contribuir simultaneamente no mesmo, editando e criando novos arquivos e permitindo que os mesmos possam existir sem o risco de suas alterações serem sobrescritas.

Se não houver um sistema de versão, imagine o caos entre duas pessoas abrindo o mesmo arquivo ao mesmo tempo. Uma das aplicações do git é justamente essa, permitir que um arquivo possa ser editado ao mesmo tempo por pessoas diferentes. Por mais complexo que isso seja, ele tenta manter tudo em ordem para evitar problemas para nós desenvolvedores.

* Git x Github

Github é um site onde você pode subir seus projetos e compartilhar com o mundo. E você vai subir eles lá usando o Git.  
A grande maioria dos projetos open source estão hospedados no Github, inclusive o código do Git está lá no Github também.  
Você pode usar o Github como portifólio do seu código e outras pessoas podem ver seus projetos e baixá-los. 
Dá pra participar de projetos open source e seguir outros desenvolvedores conhecidos por lá pra ver o que eles estão fazendo.  É tipo uma rede social para pessoas que programam :)  

Existem outros sites onde você pode subir seus projetos com Git, como o Gitlab e o Bitbucket.

Veja algumas empresas que usam o github!  
[Blizzard](https://github.com/Blizzard)  
[Twitter](https://github.com/twitter)  
[Facebook](https://github.com/facebook)  
[Google](https://github.com/google)  


[Colinha de Comandos!](https://github.com/carolvicente/minicurso-git-ft/blob/master/Git-SheetCheet.pdf)

# Vamos começar!

### Configurações Iniciais

* Cadastro no Github  https://github.com/
* Install Git no Desktop   https://git-scm.com/downloads
* Configuração do Git : 
	git config --[option] user.name "seu_nome"    
	git config --[option] user.email "seu email"   

	option : global ou local . 

### Criando um Projeto no Git

* Criação Repositório 
* Adicionar Colaboradores 
* git clone 
 
 
### Git Status 

![git status](https://git-scm.com/figures/18333fig0201-tn.png)

- Untracked :
Arquivo não mapeado pelo Git.  
O Git está vendo um arquivo que não existia na última captura (commit);  
Git não vai incluí-lo nas suas capturas de commit até que você o diga explicitamente que assim o faça.  

- Unmodified : 
Nenhum arquivo foi modificado na branch atual.  

- Modified : 
Há arquivos modificados na branch atual.  

- Staged : 
O Arquivo foi selecionado para o próximo commit.  

* git status 

### Criação de Branches 


O Git permite criar uma linha independente de desenvolvimento no seu projeto. Isto permite alterações em partes específicas do software sem comprometer o restante do projeto. Essas linhas independentes são chamadas de branches. 

* Criar nova branch :
git branch testing   

* Mudar de branch   
git checkout "nome_da_branch" . 

* Tudo em um : ou git checkout -b "nome_da_nova_branch" . 

### Criação de um Commit

Um commit pode ser interpretado como um pacote de modificações!  
git add * ou git add  
git commit  
git commit amend    
git push 

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
Atualizem todas as branches.  
Em suas branches, cada um deve editar o mesmo arquivo.  
X colega 1 deve commitar, e mergear suas mudanças na master.  
X colega 2 deve ir na master, atualizar ela, e ir de volta para a sua branch.  
 Editar esse arquivo “não atualizado”, commitar, e antes do push, realizar um merge com a master.  
BOOM!  
Vamos pro VsCode visualizar!  
