# 🚀 Projeto Exemplo com Git

Bem-vindo ao repositório! Este é um projeto de exemplo para demonstrar o uso básico do Git e GitHub.

## 🛠️ Tecnologias Usadas

- Git
- GitHub
- Markdown

### 📁 Estrutura do Projeto

### Adicionando conteúdo remotamente

---

# 🚀 Lab Prático: Git Básico com GitHub

Repositório criado para demonstrar o uso prático do Git e GitHub através de exercícios hands-on. Este projeto foi desenvolvido como parte do curso de DevOps Automation.

## 📋 Sobre o Projeto

Este repositório documenta um lab completo de Git, abordando desde instalação e configuração até conceitos avançados como branches, pull requests, tags e automação de comandos.

## 🛠️ Tecnologias Utilizadas

- **Git** - Sistema de controle de versão distribuído
- **GitHub** - Plataforma de hospedagem de código
- **Bash** - Automação de comandos Git
- **SSH** - Autenticação segura com GitHub

## 📚 O que foi praticado

### Fundamentos
- ✅ Instalação e configuração do Git
- ✅ Autenticação SSH com GitHub
- ✅ Clone de repositórios
- ✅ Commits e push
- ✅ Criação e merge de branches
- ✅ Pull Requests

### Conceitos Intermediários
- ✅ Tags e versionamento
- ✅ .gitignore para arquivos sensíveis
- ✅ Diff entre commits
- ✅ Repositórios remotos múltiplos
- ✅ Fetch e merge de upstream

### Automação
- ✅ Função Bash personalizada para comandos Git
- ✅ Configuração de ambiente com .bashrc
- ✅ Edição de arquivos com vi

## 🚀 Instalação

### Linux (Debian/Ubuntu)
```bash
sudo apt update
sudo apt install git -y
```

### macOS (Homebrew)
```bash
brew install git
```

### Windows
Baixe em: https://git-scm.com/download/win

### Verificar instalação
```bash
git --version
```

## ⚙️ Configuração Inicial
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

### Configurar SSH
```bash
# Gerar chave SSH
ssh-keygen -t ed25519 -C "seu@email.com"

# Copiar chave pública
cat ~/.ssh/id_ed25519.pub

# Adicionar em: https://github.com/settings/keys
```

## 📖 Comandos Básicos

### Clonar repositório
```bash
git clone git@github.com:seu-usuario/repositorio.git
cd repositorio
```

### Adicionar e commitar
```bash
git add .
git commit -m "Descrição das alterações"
git push
```

### Criar branch
```bash
git checkout -b nova-feature
```

### Fazer merge
```bash
git checkout main
git merge nova-feature
git push
```

## 🏷️ Versionamento com Tags
```bash
# Criar tag
git tag v1.0.0

# Enviar tag
git push origin v1.0.0
```

## 🔧 Automação: Função Git Personalizada

Esta função automatiza `git add`, `commit` e `push` em um único comando.

### Criar a função
```bash
# Criar pasta
mkdir -p ~/functions

# Criar arquivo de função
vi ~/functions/functions
```

Adicione o seguinte conteúdo:
```bash
function gitpush() {
    git add .
    git commit -m "$1"
    git push
}
```

### Configurar .bashrc
```bash
vi ~/.bashrc
```

Adicione ao final:
```bash
source ~/functions/functions
```

### Recarregar configuração
```bash
source ~/.bashrc
```

### Usar a função
```bash
gitpush "Minha mensagem de commit"
```

## 📁 Estrutura do Projeto
```
.
├── README.md           # Este arquivo
└── projeto.md          # Arquivo de exemplo criado no lab
```

## 🎯 Boas Práticas Aplicadas

- Commits atômicos e descritivos
- Uso de branches para features
- Pull Requests para code review
- Tags para versionamento semântico
- Autenticação SSH ao invés de HTTPS
- Automação de tarefas repetitivas

## 🔗 Links Úteis

- [Documentação Git](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials)

## 📝 Licença

Este projeto é de código aberto e está disponível para fins educacionais.

## ✍️ Autor

Desenvolvido como parte do aprendizado em DevOps Automation.

---

**#Git #GitHub #DevOps #ControlDeVersao #Automacao #Bash #SSH**
