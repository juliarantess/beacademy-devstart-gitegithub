# Conhecendo Git e GitHub

Praticando comandos básicos apresentados ao longo do curso **Versionamento de Projetos: Git e GitHub** do programa **[DevStart Paylivre](https://www.beacademy.com.br/devstartpaylivre/)** em conjunto com a **be.academy**.

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

## Git — Configuração inicial
Configure as credenciais do Git, assim será possível identificar os usuários responsáveis pelas alterações no projeto.
```bash
  git config --global user.name "Your name"
  git config --global user.email "Your e-mail"
```

## Git — Comandos