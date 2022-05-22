# Conhecendo Git e GitHub

Prática de comandos básicos apresentados no curso **Versionamento de Projetos: Git e GitHub** do programa **[DevStart Paylivre](https://www.beacademy.com.br/devstartpaylivre/)** em conjunto com a Be Academy.

## Instalação do Git no Linux Ubuntu
Execute os comandos abaixo no terminal
```bash
  # Adicione o PPA para download da versão estável mais recente do Git
  sudo add-apt-repository ppa:git-core/ppa
  sudo apt update
  sudo apt install git
```

Verifique a versão instalada do Git
```bash
  git --version
```

## Git
### Configuração inicial
Configure as credenciais do Git, assim será possível identificar os usuários responsáveis pelas alterações no projeto
```bash
  git config --global user.name "Your name"
  git config --global user.email "Your e-mail"
```

### Comandos iniciais
`git init` — Inicializa um repositório local do Git.

`git status` — Exibe o status dos arquivos do repositório local.

`git add .` — Adiciona todos os arquivos do repositório local ao versionamento, preparando-os para o commit.

`git rm --cached <nome_do_arquivo>` — Remove o arquivo do versionamento.

`git commit -m <adicionar_mensagem_commit>` — Registra as alterações no arquivo e envia para a plataforma de versionamento.

`git log` — Exibe informações sobre os commits realizados.

### Branches
`git branch` — Lista as branches criadas no repositório local e a branch atual.

`git branch <nome_da_branch>` — Cria uma branch nova.

`git checkout <nome_da_branch>` — Alterna entre uma branch e outra.

`git checkout -b <nome_da_branch>` — Cria uma branch nova, acessando-a em seguida.

`git branch -d <nome_da_branch>` — Remove uma branch.

`git merge <nome_da_branch>` — Unifica os arquivos das branches.

## GitHub — Repositório remoto
### Configurando a chave SSH
Através do protocolo SSH (Secure Shell), é possível se conectar a servidores e serviços remotos. A chave SSH permite conectar-se ao GitHub inserindo dados de acesso uma única vez.

Execute o comando abaixo no terminal

```bash
  ssh-keygen -t ed25519 -C "your_email@example.com"
```
Após inserir uma senha, busque pelo caminho indicado no terminal, abra o arquivo **.pub** e copie a chave.

No GitHub, em [SSH keys](https://github.com/settings/keys), adicione uma nova chave.

### Publicando no repositório remoto
Chave SSH configurada, é possível clonar o repositório remoto pelo protocolo SSH.

`git clone <link_do_repositorio>` — Realiza o download de um repositório remoto do GitHub para seu repositório local.

`git remote -v` — Lista os repositórios remotos.

`git push` — Envia as alterações realizadas no repositório local para o repositório remoto.
