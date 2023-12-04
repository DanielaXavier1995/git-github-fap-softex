# Olá devs 🖐👩🏽‍💻👨🏽‍💻✨

Estamos aqui para compartilhar um pouco de conhecimento sobre os nossos queridos amigos Git e GitHub 🤩

</div align="middle">
<h1 align="center">

<img align="middle" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="80" height="80"/> <img align="middle" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="80" height="80"/> 

</h1>
</div>

## 🛠️ Primeiros Passos: 
### Git x GitHub:
 
                     🤔 E AI? TODOS SABEM O QUE É E QUAIS AS DIFERENÇAS ENTRE O COMBO GIT E GITHUB? 🤔 

  #### Por que esse combo é tão importante?
  * Versionamento;
  * Backup;
  * Colaboração entre pessoas/equipes;
  * Portfólio;
      
  #### Git:
  * Servidor para versionamento de código;
  * Criado pelo time da Linux;
  
  #### GitHub:
  * Plataforma para hospedagem de código;
  * Permite a colaboração entre pessoas;
  * Interface amigável;
  
### Instalação:
* Link para instalação:

                                             https://git-scm.com/download/win
  
### Configuração:
* Comandos para configuração do usuário:
  
1) Configurando o nome de usuário:
   
                             git config --global user.name "Mesmo nome de usuário do GitHub"
    
3) Configurando o email do usuário:
   
                                 git config --global user.email "abcdef@exemplo.br"
   
5) Verificar informações:
   
                                              git config --list
   
### Autenticação via chave SSH:
* Configuração da chave SSH:

1) Vá no menu de opções e click em: settings
2) Dentro de Settings encontre: SSH and GPG Keys
3) Entre no link: generating SSH keys
* Gerando a chave SSH:

      https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
  
4) Adicione a chave SSH ao gitHub > New SSH key
     
![ssh](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/1451e0d8-f013-41fd-8161-63f5e818ffaf)

### Repositório Local x Repositório Remoto:

* REPOSITÓRIO LOCAL -> Pasta no computador -> .git -> palavra reservada MAIN
* REPOSITÓRIO REMOTO -> Repositório do seu próprio GitHub -> palavra reservada ORIGIN (substitui uma URL)
* REPOSITÓRIO REMOTO -> Repositório do GitHub atrelado a outra conta (fork para sua conta) -> palavra reservada UPSTREAM 

![veremos](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/0f36b40f-9c26-4db1-8ff5-6d7e190fa5ce)

### Estados dos arquivos:

                              🤔 ALGUÉM CONHECE COMO FUNCIONA OS ESTADOS DOS ARQUIVOS NO GIT? 🤔 

<h1 align="center">
 
![fluxo git](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/c67422cd-0b72-473d-80d6-cd482c36295b)

</h1>

* Comandos x Mudanças de estado do arquivo:

![fluxo 2](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/e65afa4d-8327-4d99-a3bd-bc2b4d8ae507)



### Comandos para iniciar o versionamento:

   #### 1° OPÇÃO: Criar e Linkar o repositório local ao remoto

   1) Criar o repositório local (pasta) com um arquivo;
   2) Criar um repositório git:
      
                                               git init
      
   4) Linkar o repositório local ao remoto:
      
                           git remote add origin <LINK DO REPOSITÓRIO REMOTO>

                                            git remote
      
   6) Preparar o commit:

                                          git add <Nome do arquivo> ou git add .

                                                      git status
      
                                            git commit -m "NOME DO COMMIT"

                                                      git status
      
   8) Subir o commit:

                                             local para o remoto:  git push origin main

                                                 remoto para o local:  git pull
      
      
   #### 2° OPÇÃO: Baixar um repositório remoto

   1) clonar um repositório remoto para o repositório local:

                                    git clone <URL DO REPOSITÓRIO>

                                             git remote
      
### Outros comandos importantes:

1) Visualizar histórico de commits:
   
                                              Histórico de commits completo: git log
   
                                            Histórico de commits resumido:  git reflog
   
3) Restaurar commits:

* Voltar para estados anteriores:

                                volta para o estado modificado:     git restore <Nome do arquivo>

                                volta para área de staged:       git restore --staged <Nome do arquivo>
  
* Voltar para commits anteriores: ?????//?

                           volta para o commit indicado:      git reset --hard <hash do commit>

### Trabalhando com Branchs: ????????
   
### Vamos nos conectar?
[![LinkedIn](https://img.shields.io/badge/LinkedIn-000?style=for-the-badge&logo=linkedin&logoColor=0E76A8)](https://www.linkedin.com/in/dani-xavier/)
[![Discord](https://img.shields.io/badge/Discord-000?style=for-the-badge&logo=discord)](https://www.discord.com/in/DanielaXavier#0328/)
   



