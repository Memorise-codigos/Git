[⬅Volta](https://memorise-codigos.github.io/Morise-codigo/)
# Introdução
O Git é um sistema de controle de versão de arquivos de código aberto, usado para gerenciar projetos de software e colaboração em equipe. Ele foi criado por Linus Torvalds em 2005 e é amplamente utilizado por equipes de desenvolvimento em todo o mundo. O Git permite que os desenvolvedores rastreiem as alterações em seus arquivos de código-fonte, trabalhem em equipe em um mesmo projeto e revertam facilmente para versões anteriores do código. Neste manual, você aprenderá os comandos Git mais comuns e como usá-los.
# Instalação do Git
Antes de começar a usar o Git, você precisa instalá-lo em seu computador. O Git pode ser instalado em sistemas operacionais Windows, Mac e Linux. Você pode baixar a última versão do Git [Clicando aqui](https://git-scm.com/downloads). Depois de baixar o instalador, basta seguir as instruções na tela para instalá-lo em seu computador.
# Configuração do Git
Antes de começar a usar o Git, você precisa configurá-lo com seu nome de usuário e endereço de e-mail. Essas informações serão usadas para registrar as alterações que você fizer em seus arquivos.

Para configurar seu nome de usuário, execute o seguinte comando:

- `git config --global user.name "Seu Nome"`

Para configurar seu endereço de e-mail, execute o seguinte comando:
- `git config --global user.email "exemplo@gmail.com"`
# Iniciando um Repositório Git
Para iniciar um novo repositório Git, basta navegar até o diretório do seu projeto e executar o seguinte comando:
- `git init`

Isso irá criar um novo repositório Git em seu diretório. O Git agora estará pronto para controlar as alterações em seus arquivos.
Se você deseja clonar um repositório Git existente, use o comando git clone seguido da URL do repositório:
- `git clone https://github.com/seu-usuario/seu-repositorio.git`
# Adicionando arquivos ao controle de versão
Antes de começar a controlar as alterações em seus arquivos, você precisa adicionar os arquivos ao controle de versão Git. Para fazer isso, use o comando `git add` seguido do nome do arquivo que você deseja adicionar.

Adicionar um arquivo específico:
- `git add nome-do-arquivo`

Adicionar todos os arquivos no diretório atual:
- `git add .`
# Commit de Alterações
Quando você adiciona arquivos ao controle de versão Git, as alterações não são registradas automaticamente. Para registrar suas alterações, você precisa fazer um commit. Um commit é um registro de todas as alterações que você fez em seus arquivos.

Para fazer um commit, use o comando git commit seguido de uma mensagem que descreva as alterações que você fez:
- `git commit -m "Sua mensagem de commit aqui"`

A mensagem de commit deve descrever claramente as alterações que você fez. Isso ajudará outros membros da equipe a entender o que foi alterado no código.
# Ramificação (Branching)
As ramificações (branches) são cópias do código em um determinado momento, permitindo que você faça alterações e experimente sem afetar o código principal. Isso é especialmente útil quando você está trabalhando em grandes projetos com várias pessoas.

Para criar uma nova ramificação, use o comando git branch seguido do nome da ramificação:
- `git branch nome-da-ramificacao`

Para mudar para a nova ramificação, use o comando git checkout seguido do nome da ramificação:
- `git checkout nome-da-ramificacao`

Você também pode criar e mudar para uma nova ramificação em um único comando usando git checkout -b:
- `git checkout -b nome-da-ramificacao`

Depois de fazer alterações em uma ramificação, você pode mesclar as alterações na ramificação principal usando o comando git merge:
- `git checkout ramificacao-principal`
- `git merge nome-da-ramificacao`
# Trabalhando com Repositórios Remotos
O Git permite que você trabalhe em colaboração com outros desenvolvedores, compartilhando o código por meio de um repositório remoto. Existem várias plataformas de hospedagem de repositórios Git, como GitHub, GitLab e Bitbucket.

Para adicionar um repositório remoto, use o comando git remote add seguido do nome do repositório e da URL do repositório:
- `git remote add nome-do-repositorio URL-do-repositorio`

Você pode verificar quais repositórios remotos estão configurados em seu projeto usando o comando git remote:
- `git remote`

Para enviar suas alterações para o repositório remoto, use o comando git push seguido do nome do repositório remoto e da ramificação em que você está trabalhando:
- `git push nome-do-repositorio nome-da-ramificacao`

Para baixar as alterações mais recentes do repositório remoto, use o comando git pull seguido do nome do repositório remoto e da ramificação em que você está trabalhando:
- `git pull nome-do-repositorio nome-da-ramificacao`
# Desfazendo Alterações
O Git permite que você desfaça alterações em seus arquivos, mesmo depois de fazer um commit. Para desfazer as alterações em um arquivo, use o comando git checkout seguido do nome do arquivo:
- `git checkout nome-do-arquivo`

Isso reverterá o arquivo para a versão mais recente que foi commitada.

Se você deseja desfazer um commit, use o comando git revert seguido do hash do commit que deseja reverter:
- `git revert hash-do-commit`

Isso criará um novo commit que desfaz as alterações do commit anterior
# Conclusão
O Git é uma ferramenta poderosa e essencial para qualquer desenvolvedor de software. Com os comandos descritos neste manual, você deve ter uma boa compreensão do básico do Git. No entanto, há muito mais a ser explorado e aprendido, então não deixe de ler a documentação oficial do Git e experimentar os comandos por conta própria. Com prática e experiência, você se tornará um usuário avançado do Git em pouco tempo.
