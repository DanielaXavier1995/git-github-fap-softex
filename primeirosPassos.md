## 🛠️ Primeiros Passos:

### Git x GitHub:

                          🤔 E AI? TODOS SABEM O QUE É E QUAIS AS DIFERENÇAS ENTRE O COMBO GIT E GITHUB? 🤔

#### Por que esse combo é tão importante?

- Versionamento;
- Backup;
- Colaboração entre pessoas/equipes;
- Portfólio;

#### Git:

- Servidor para versionamento de código;
- Criado pelo time da Linux;

#### GitHub:

- Plataforma para hospedagem de código;
- Permite a colaboração entre pessoas;
- Interface amigável;

### Instalação:

- Link para instalação:

                                                 https://git-scm.com/download/win

### Configuração:

- Comandos para configuração do usuário:

1.  Configurando o nome de usuário:

                                   git config --global user.name "Mesmo nome de usuário do GitHub"

2.  Configurando o email do usuário:

                                        git config --global user.email "abcdef@exemplo.br"

3.  Verificar informações:

                                                     git config --list

### Autenticação via chave SSH:

- Configuração da chave SSH:

1. Vá no menu de opções e click em: settings
2. Dentro de Settings encontre: SSH and GPG Keys
3. Entre no link: generating SSH keys

- Gerando a chave SSH:

      https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

- Adicione a chave SSH ao gitHub > New SSH key

![ssh](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/1451e0d8-f013-41fd-8161-63f5e818ffaf)

### Repositório Local x Repositório Remoto:

- REPOSITÓRIO LOCAL -> Pasta no computador -> .git -> palavra reservada MAIN
- REPOSITÓRIO REMOTO -> Repositório do seu próprio GitHub -> palavra reservada ORIGIN (substitui uma URL)
- REPOSITÓRIO REMOTO -> Repositório do GitHub atrelado a outra conta (fork para sua conta) -> palavra reservada UPSTREAM

![veremos](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/0f36b40f-9c26-4db1-8ff5-6d7e190fa5ce)

### Estados dos arquivos:

                              🤔 ALGUÉM CONHECE COMO FUNCIONA OS ESTADOS DOS ARQUIVOS NO GIT? 🤔


<h1 align="center">
 
![fluxo git](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/c67422cd-0b72-473d-80d6-cd482c36295b)

</h1>

- Comandos x Mudanças de estado do arquivo:

![fluxo 2](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/e65afa4d-8327-4d99-a3bd-bc2b4d8ae507)

### Comandos para iniciar o versionamento:

#### 1° OPÇÃO: Criar e Linkar o repositório local ao remoto

1.  Criar o repositório local (pasta) com um arquivo;
2.  Criar um repositório git:

                                                           git init

3.  Linkar o repositório local ao remoto:

                                      git remote add origin <LINK DO REPOSITÓRIO REMOTO>

                  Mostra todos os repositórios remotos atrelados ao meu repositório local:  git remote

4.  Preparar o commit:

                                            git add <Nome do arquivo> ou git add .

                                                         git status

                                               git commit -m "NOME DO COMMIT"

                                                        git status

5.  Subir o commit:

                                            Local para o remoto:  git push origin main

                                                 Remoto para o local:  git pull

#### 2° OPÇÃO: Baixar um repositório remoto

1.  clonar um repositório remoto para o repositório local:

                                               git clone <URL DO REPOSITÓRIO>

                                                        git remote

### Outros comandos importantes:

1.  Visualizar histórico de commits:

                                               Histórico de commits completo: git log

                                             Histórico de commits resumido:  git reflog

2.  Restaurar commits:

- Voltar para estados anteriores:

                                 Volta para o estado modificado:     git restore <Nome do arquivo>

                              Volta para área de staged:       git restore --staged <Nome do arquivo>

- Voltar para commits anteriores:

             Volta para o commit indicado, ignorando tudo oque foi feito anteriormente (apaga todas as modificações):
                                           git reset --hard <hash do commit>

        Volta para o commit indicado (retorna as modificações para a área de stage permitindo que possam ser commitadas novamente):
                                           git reset --soft <hash do commit>

### Trabalhando com Branchs:

                                               🤔 O QUE SÃO AS BRANCHS? 🤔

<h1 align="center">

![branchs](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/c19b7f5e-b9f5-4d54-a609-71913b27d189)

</h1>

### Comandos para trabalhar com branchs:

OBS 1: A branch sempre será criada a partir da branch em que voçê está trabalhando no momento, como no exemplo da imagem acima,
estando na branch master/main posso criar a branch de desenvolvimento, a partir desta posso criar branchs para as funcionalidades
que estou desenvolvendo.

1.  Criando a branch de desenvolvimento a partir da main:

                                   Para criar e entrar na branch:   git checkout -b "develop"

2.  Subindo modificações para a branch:

                                             git push origin "nome_da_branch"

3.  Deletando branchs:

                                             git branch -d "nome_da_branch"

### Mesclando branchs:

OBS 2: Você sempre deve estar na branch pela qual quer trazer as modificações, exemplo: se você quer mesclar a branch DEVELOP com uma FEATURE
vai precisar entrar na branch DEVELOP para depois realizar o merge com a FEATURE.

1.  Entrando em DEVELOP:

                                                git checkout "develop"

2.  Merge:

                                                 git merge "feature"

### Commit semântico:

1. **docs**: referem-se a inclusão ou alteração somente de arquivos de documentação;
2. **feat**: Tratam adições de novas funcionalidades ou de quaisquer outras novas implantações ao código;
3. **fix**: Essencialmente definem o tratamento de correções de bugs;
4. **perf**: Uma alteração de código que melhora o desempenho;
5. **refactor**: Tipo utilizado em quaisquer mudanças que sejam executados no código, porém não alterem a funcionalidade final da tarefa impactada;
6. **test**: Adicionando testes ausentes ou corrigindo testes existentes nos processos de testes automatizados (TDD);
