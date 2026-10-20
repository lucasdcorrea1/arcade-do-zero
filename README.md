# 🕹️ Arcade do Zero

Monte um **fliperama bartop de 2 jogadores do zero** — impresso em 3D, com guia passo a passo,
controle das impressões e um app grátis para rodar os jogos na Raspberry Pi.

**🌐 Site: https://lucasdcorrea1.github.io/arcade-do-zero/**

Tudo é **gratuito e open source**. Sem cadastro, sem pegadinha.

---

## ⬇️ Baixar o app (RetroPie ROM Sender)

App de desktop (Windows) que navega num site de ROMs, intercepta o download e envia o jogo
direto pra sua Raspberry Pi (via SFTP), já na pasta certa do emulador — sem FileZilla, sem terminal.

- **[Baixar o portable (roda sem instalar)](https://github.com/lucasdcorrea1/arcade-do-zero/releases/latest/download/RetroPie-ROM-Sender-portable.exe)**
- **[Baixar o instalador (.exe)](https://github.com/lucasdcorrea1/arcade-do-zero/releases/latest/download/RetroPie-ROM-Sender-Setup.exe)**
- [Todas as versões (releases)](https://github.com/lucasdcorrea1/arcade-do-zero/releases)

Windows 64-bit. Os links acima **sempre apontam para a versão mais recente**.

---

## ✅ É open source — por que você pode confiar

Baixar e rodar um `.exe` da internet pede cautela, e você está certo em desconfiar.
Por isso **tudo aqui é código aberto (licença MIT)**:

- 🔓 **Leia o código antes de rodar.** O app é feito em Electron e o código-fonte completo está em
  **[arcade-games-setup/desktop-app](https://github.com/lucasdcorrea1/arcade-games-setup/tree/main/desktop-app)**. Nada é ofuscado.
- 🛠️ **Não confie no meu `.exe` — gere o seu.** Em 3 comandos você compila o mesmo app a partir do
  código (`npm install` → `npm run dist`). Aí você não depende do arquivo que eu publiquei.
- 🕵️ **Sem rastreio, sem telemetria, sem conta.** O app **não envia nada** pra servidores meus. Ele só
  conversa com (1) o site de ROMs que **você** abre e (2) a **sua** Raspberry Pi, na sua rede local.
- 💾 **Seus dados ficam só no seu PC** (IP/senha da Pi em `%APPDATA%/retropie-rom-sender/`).
- 🪪 **Licença MIT** — use, estude, modifique e distribua livremente.

### ⚠️ "O Windows protegeu o seu PC" (SmartScreen)

Como o app é gratuito e **sem assinatura digital paga**, o Windows pode mostrar um aviso azul ao abrir.
**Isso é esperado para qualquer app novo sem certificado caro — não quer dizer vírus.** Para rodar:
clique em **"Mais informações" → "Executar assim mesmo"**. Prefere não confiar no `.exe`? **Compile o seu.**

---

## 🧩 O que tem no projeto

| Parte | O que é | Link |
|------|---------|------|
| **Landing** | A vitrine do projeto | [site](https://lucasdcorrea1.github.io/arcade-do-zero/) |
| **Guia passo a passo** | Da impressão à montagem (8 etapas, renders 3D, lista de material, config do slicer) | [guia](https://lucasdcorrea1.github.io/arcade-do-zero/guia.html) |
| **Controle de impressão** | Painel pra marcar o que já imprimiu, falhas, horas e comentários por peça (229 peças) | [controle](https://lucasdcorrea1.github.io/arcade-do-zero/controle.html) |
| **App do emulador** | RetroPie ROM Sender (download acima) | [código](https://github.com/lucasdcorrea1/arcade-games-setup/tree/main/desktop-app) |

---

## 🛠️ Compilar o app você mesmo

```bash
git clone https://github.com/lucasdcorrea1/arcade-games-setup
cd arcade-games-setup/desktop-app
npm install
npm run dist     # gera o .exe em dist/
```

O resultado é o mesmo app dos downloads acima — verificável, sem surpresas.

---

## 📂 Este repositório

Contém os arquivos do **site** (servido via GitHub Pages) e os **releases** do app:

```
index.html       landing page
guia.html        guia passo a passo
controle.html    controle de impressão
assets/          imagens do site
_THUMBS/         miniaturas 3D das peças
.nojekyll        serve a pasta _THUMBS (underscore) no GitHub Pages
```

O **código-fonte do app** fica em [arcade-games-setup](https://github.com/lucasdcorrea1/arcade-games-setup).

---

## 📜 Licença

MIT — livre para usar, modificar e compartilhar. Baixe apenas jogos que você tem o direito de usar.
