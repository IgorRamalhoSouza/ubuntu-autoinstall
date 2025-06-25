# Ubuntu Autoinstall

Um projeto para automatizar a instalação do Ubuntu 24.04 com minhas configurações pessoais preferidas, removendo bloatware e personalizando o sistema.

## 🇧🇷 Versão em Português

### Como usar

1. Baixe a ISO oficial do Ubuntu 24.04
2. Grave a ISO em um pendrive USB (usando Balena Etcher, Rufus ou similar)
3. Copie os arquivos `autoinstall.yaml` e `ubuntu-debullshit.sh` para a raiz do pendrive
4. Inicie o computador pelo pendrive
5. A instalação começará automaticamente e pode pedir conexão Wi-Fi se necessário

### O que cada arquivo faz?

#### autoinstall.yaml
- Configura a instalação automática do Ubuntu
- Define usuário, senha, idioma e timezone
- Particiona o disco com LUKS encryption usando TPM (se disponível)
- Instala todos os programas que eu uso (Chrome, Steam, VS Code, etc)
- Configura LVM como gerenciador de volumes

#### ubuntu-debullshit.sh
Script que roda após a instalação para:
- Remover Snap e todo rastro dele do sistema
- Instalar Flatpak e configurar Flathub
- Remover telemetria e relatórios do Ubuntu
- Desativar anúncios no terminal
- Instalar Firefox direto da Mozilla
- Configurar GNOME Vanilla (mais limpo que o padrão do Ubuntu)
- Aplicar temas ADW-GTK3 e ícones MoreWaita
- Muitas outras otimizações

## 🇺🇸 English Version

### How to use

1. Download official Ubuntu 24.04 ISO
2. Flash it to a USB drive (using Balena Etcher, Rufus or similar)
3. Copy both `autoinstall.yaml` and `ubuntu-debullshit.sh` to the root of the USB
4. Boot from the USB drive
5. Installation will start automatically and may ask for Wi-Fi connection if needed

### What each file does?

#### autoinstall.yaml
- Configures Ubuntu automated installation
- Sets user, password, language and timezone
- Partitions disk with LUKS encryption using TPM (if available)
- Installs all my preferred apps (Chrome, Steam, VS Code, etc)
- Configures LVM as volume manager

#### ubuntu-debullshit.sh
Post-install script that:
- Removes Snap and all its traces from system
- Installs Flatpak and configures Flathub
- Removes Ubuntu telemetry and reporting
- Disables terminal ads
- Installs Firefox directly from Mozilla
- Sets up Vanilla GNOME (cleaner than default Ubuntu)
- Applies ADW-GTK3 themes and MoreWaita icons
- Many other optimizations

---

Feito com ❤️ por [Seu Nome] - Personalizando Ubuntu desde [ano]