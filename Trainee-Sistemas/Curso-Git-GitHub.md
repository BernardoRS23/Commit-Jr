# #1 Introdução

## Principais Benefícios do Git

- Histórico detalhado de versões: registro de cada alteração feita no código;
- "Segurança" para testes: permite voltar em versões anteriores caso aconteça algum bug;
- Colaboração em equipe: permite trabalhar com mais pessoas simultaneamente sem bagunçar o código original do projeto.

## Principais Benefícios do GitHub

- Oferece as funcionalidades do Git;
- Backup remoto: projetos salvos na nuvem, evitando perda de dados se o computador estragar;
- "Rede Social": funcione como uma vitrine para seus projetos, ajudando a comprovar suas habilidades para o mercado de trabalho, compartilhamento fácil de projetos e permite outros que outros usuários colaborem com seu código.

# #2 Conceitos Básicos do Git

- **Repositório:** rastreia todas as mudanças feitas no arquivos do seu projeto, construindo um histórico ao longo do tempo
- **Commit:** um marco histórico no seu projeto, como se fosse um "save" nos jogos de videogame. Te permite "voltar" no tempo para consultar diferentes versões importantes do seu projeto.
- **Branch:** linha de desenvolvimento independente que permite alterar códigos sem mexer na versão principal do projeto.

# #3 Instalação do Git e alguns comandos no Terminal

- ls: listar arquivos e diretórios do diretório atual
- cd {nome-do-diretorio}: acessar diretório
- cd..: voltar para o diretório anterior, "pai"
- ni {nome-arquivo}: criar arquivo
- rm {nome-arquivo}: remover arquivo
- mkdir {nome-diretório}: criar novo diretório
- nano {nome-do-arquivo} (não instalado no Windows): editor de texto para terminal
- cat {nome-do-arquivo} (não instalado no Windows): exibir conteúdo do arquivo

# #4 Criando repositórios

Comando utilizados:
-  git --version //versão do git, confirma instalação;
-  mkdir projeto-1 //cria o diretório projeto-1;
-  mkdir projeto-02 //cria o diretório projeto-02 -> nome diferente propositalmente;
-  mv projeto-02 projeto-2 //mv renomeia ou move o arquivo/diretório de lugar;
-  cd projeto-1 //entra no diretório projeto-1;
-  git init //cria repositório;
-  ls //inicialmente, não resulta em nada -> o arquivo .git é ocultado pelo sistema operacional;
-  ls -Force //agora, lista itens ocultados (.git);
-  cd ../projeto-2 //volta para o diretório "pai" e entra para projeto-2;
-  ni index.html //cria arquivo;
-  ni style.css //cria arquivo;
-  git init //cria repositório -> nesse momento o nome dos arquivos criados fica verde, esses arquivos agora estão no estado modificado;

# #5 Colocando arquivos no stage

1. Continuamos a partir dos arquivos/diretórios/repositórios criados na aula #4.
2. Inicialmente, na pasta projeto-1, criamos o arquivo index.html (ni index.html) e usamos o comando git add index.html para colocar esse arquivo no stage.
3. Com o comando git status, conseguimos observar que o arquivo foi colocado no stage.
4. Para tirar o arquivo do stage, utilizamos o comando git rm --cached index.html.
--
5. Agora na pasta projeto-2, com dois arquivos criados, usamos git add . para adicionarmos todos os arquivos no stage de uma vez.

# #6 primeiro COMMIT.

Após colocar o arquivo no stage, para dar commit utilizamos o comando git commit -m "mensagem";
Para conferir o histórico de commit's, usamos o comando git log ou git log --oneline (para a versão condensada);
