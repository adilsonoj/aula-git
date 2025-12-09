# Git e GitHub - Guia Básico

Este documento serve como uma introdução rápida aos conceitos fundamentais de Git e GitHub, incluindo sua história e comandos essenciais.

## 🧐 O que é?

### Git
O **Git** é um sistema de controle de versão distribuído, gratuito e de código aberto. Ele foi projetado para lidar com tudo, desde projetos pequenos até muito grandes, com velocidade e eficiência.
- **Função Principal:** Rastrear mudanças no código-fonte, permitindo que múltiplos desenvolvedores trabalhem juntos sem sobrescrever o trabalho uns dos outros.

### GitHub
O **GitHub** é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão usando o Git.
- **Função Principal:** Facilitar a colaboração. Ele oferece uma interface web para o Git, além de funcionalidades como rastreamento de bugs, solicitações de funcionalidades (feature requests), gerenciamento de tarefas e wikis para cada projeto.

---

## 📜 Um Pouco de História

### A Origem do Git (2005)
O Git foi criado por **Linus Torvalds** (o mesmo criador do Linux). A motivação surgiu após a equipe de desenvolvimento do kernel do Linux perder a licença gratuita do sistema de controle de versão que usavam na época (BitKeeper). Linus queria um sistema que fosse rápido, distribuído e seguro contra corrupção de dados. Ele desenvolveu a primeira versão do Git em poucas semanas.

### O Surgimento do GitHub (2008)
O GitHub foi lançado em abril de 2008 por Tom Preston-Werner, Chris Wanstrath e PJ Hyett. A ideia era simplificar o compartilhamento de código e a colaboração. Rapidamente se tornou a maior plataforma de código aberto do mundo. Em 2018, a Microsoft adquiriu o GitHub, mantendo-o como uma plataforma aberta para desenvolvedores.

---

## 🚀 Comandos Básicos

Aqui estão os comandos que você usará em 90% do tempo:

### 1. Configuração Inicial
Antes de começar, você precisa se identificar para o Git:
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"
```

### 2. Iniciando um Projeto
```bash
# Inicializa um repositório Git em uma pasta existente
git init

# Ou baixa um repositório existente do GitHub
git clone https://github.com/usuario/projeto.git
```

### 3. O Ciclo de Vida do Commit (Salvar Alterações)
```bash
# Verifica o estado dos arquivos (o que mudou?)
git status

# Adiciona arquivos à área de preparação (Stage)
git add nome_do_arquivo.txt   # Um arquivo específico
git add .                     # Todos os arquivos modificados

# Salva as mudanças no histórico (Commit)
git commit -m "Uma mensagem clara sobre o que foi alterado"
```

### 4. Sincronizando com o GitHub
```bash
# Envia seus commits locais para o repositório remoto (Upload)
git push origin main

# Atualiza seu repositório local com as mudanças do remoto (Download)
git pull origin main
```

### 5. Histórico e Logs
```bash
# Mostra o histórico de commits
git log

# Mostra o histórico de forma resumida e gráfica
git log --oneline --graph --all
```

### 6. Branches (Ramificações)
Branches permitem trabalhar em novas funcionalidades sem afetar o código principal.
```bash
# Cria uma nova branch
git branch nome-da-feature

# Muda para a branch
git checkout nome-da-feature
# ou (comando mais moderno)
git switch nome-da-feature

# Funde a branch atual com outra (Merge)
git merge nome-da-feature
```

---

> "Talk is cheap. Show me the code." — Linus Torvalds