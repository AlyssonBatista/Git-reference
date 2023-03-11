# Introdução 

> Primeiro de tudo é abrir a pasta onde você quer desenvolver seu projeto, clicar com o botão direito e clicar em "abrir com **git bash**. 
>
>*OBS*: Provavelmente tem uma maneira de acessar uma pasta direto do terminal, mas, eu ainda não sei como fazer isso.



|    **comando**     |         **O que faz**             |       
|----------------|-------------------------------|
|```Mkdir```|Cria uma pasta em um local específico.|
|```cd (nome do projeto)```| Abre a pasta projeto ```(nome do projeto)```|
|```cd..```| Volta para o diretório anterior ao atual|
|```git init```|Inicia o versionamento na pasta projeto|
|```touch index.html```|  Cria um arquivo na pasta projeto, se caso você esteja na pasta projeto|
|```ls -la ```|Mostra os arquivos da pasta projeto|
|```ll```|Mostra o número de arquivos da pasta projeto|
|```git status```|Verifica o status atual do meu repositório|


# Adicionando arquivos e fazendo as configurações iniciais do git

   ![alt text](https://github.com/AlyssonBatista/Git-reference/blob/master/est%C3%A1gios.png)

|    **comando**     |         **O que faz**             |       
|----------------|-------------------------------|
| ```git add index.html ```|Adiciona o arquivo index ao staging area, ele não está no git ainda|
|```git add```|Adiciona todos os arquivos ao staging area|
|```git config --global user.name "O seu nome"```|Configura o git com o meu nome ***(essa etapa só precisa ser feita uma vez, com isso todos os projetos que você versionar terão o seu nome)***.|
|```git config --global user.email "digite o seu email aqui"```|Configura o git com meu email ***(essa etapa só precisa ser feita uma, com isso todos os projetos que você versionar terão o seu email)***.|
|```git config --list```| Lista todas as configurações que eu tenho no meu git|
|```git commit -m "Adicionei o arquivo index.html"```|Faz com que o arquivo saia da staging area e vá para  .git directory|


