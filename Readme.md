# Introdução 

> Primeiro de tudo é abrir a pasta onde você quer desenvolver seu projeto, clicar com o botão direito e clicar em "abrir com **git bash**. 
>
>*OBS*: Provavelmente tem uma maneira de acessar uma pasta direto do terminal, mas, eu ainda não sei como fazer isso.



|    **Comando**     |         **O que faz**        |       
|--------------------|------------------------------|
|```Mkdir```|Cria uma pasta em um local específico.|
|```cd (nome do projeto)```| Abre a pasta projeto ```(nome do projeto)```.|
|```cd..```| Volta para o diretório anterior ao atual.|
|```git init```|Inicia o versionamento na pasta projeto.|
|```touch index.html```|  Cria um arquivo na pasta projeto, se caso você esteja na pasta projeto.|
|```ls -la ```|Mostra os arquivos da pasta projeto.|
|```ll```|Mostra o número de arquivos da pasta projeto.|
|```git status```|Verifica o status atual do meu repositório.|


# Adicionando arquivos e fazendo as configurações iniciais do git

   ![alt text](https://github.com/AlyssonBatista/Git-reference/blob/master/est%C3%A1gios.png)
   
|    **Comando**     |         **O que faz**        |       
|--------------------|------------------------------|
| ```git add index.html ```|Adiciona o arquivo index ao staging area, ele não está no git ainda.|
|```git add .```|Adiciona todos os arquivos ao staging area.|
|```git add --all```| Todas as ações que estiverem no working directore são adicionadas para o staging area. Funciona da mesma forma que ```git add .```. |
|```git config --global user.name "O seu nome"```|Configura o git com o meu nome ***(essa etapa só precisa ser feita uma vez, com isso todos os projetos que você versionar terão o seu nome)***.|
|```git config --global user.email "digite o seu email aqui"```|Configura o git com meu email ***(essa etapa só precisa ser feita uma, com isso todos os projetos que você versionar terão o seu email)***.|
|```git config --list```| Lista todas as configurações que eu tenho no meu git|
|```git commit -m "Adicionei o arquivo index.html"```|Faz com que o arquivo saia da staging area e vá para .git directory.|

# Ver log de arquivos

|    **Comando**     |         **O que faz**        |       
|--------------------|------------------------------|
|```git log```| Vai retornar um histórico de todos os commits que eu fiz(**para sair da tela do git log digite q**).|
|```git diff```| Mostra todas as mudanças que eu fiz no código do meu arquivo. Compara os arquivos do working directory com staging area.|
|```git diff index.html```|Mostra as mudanças que eu fiz num arquivo específico.|
|```git diff --staged```|Mostra todas as mudanças que eu fiz no código do meu arquivo. Compara os arquivos do  staging area  com  .git directory.|

>OBS: Quando editamos um arquivo que já foi "commitado" ele volta para working directory . Para que ele seja versionado novamente ele precisa voltar para staging area e depois “commitamos” de novo para .git directory.

# Voltando no tempo

|    **Comando**     |         **O que faz**        |       
|--------------------|------------------------------|
|```git log --name-status```|Mostra todos os commits e os arquivos adicionados modificados e os nomes dos arquivos.|
|```git diff 0293135ab070db24b3738f1402bc31f7976677d4```|Mostra o que tem no commit atual, ou commit específico, com o primeiro commit. Caso não queira todos os dígitos, só precisa copiar os 7 primeiros.|
|```git diff 5434707 68f2908```| Compara as mudanças que estão em um commit com outro.|

# Removendo arquivos 

|    **Comando**     |         **O que faz**        |       
|--------------------|------------------------------|
|```rm style.css```| Remove o arquivo do staging area ou working directory.|
| ```git rm style.css```|  Remove o arquivo do git directore.|

# Ignorando arquivos 

|    **Comando**     |         **O que faz**        |       
|--------------------|------------------------------|
|```echo "node_modules" >> .gitignore```| Cria o arquivo(pode criar manualmente no vs code) ```.gitignore``` e adicona node_modules ao ```.gitignore```. A pasta node_modules ficará oculta e não vai pertencer ao projeto.|
| ```cat .gitignore```|  Ver o que tem dentro do ```.gitignore```|
| ```vim .gitignore```|  Edita o ```.gitignore``` e adiciona algum arquivo que eu queira ocultar. Para salvar e sair digite ```:wq``` ou ```:x```ou ```:wqa```|
|```git rm -rf  node_modules/ --cached```| Remove um arquivo indesejado do working directore ou staging area sem que eu exclua da minha pasta local.|

