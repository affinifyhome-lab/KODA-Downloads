# KODA Desktop Downloads

**English** · [Português](#português)

Official public installers for **KODA Desktop** (Electron shell loading `https://kodahub.space/codex/setup`).

This repository is the **download queue** for all platforms. Only published artifacts listed below are safe to install.

---

## Release queue

| Platform | Status | File | Approx. size |
|----------|--------|------|--------------|
| **Windows** x64 | ✅ **Beta — available** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~127 MB (~121 MiB) |
| **Linux** x64 | ⚠️ **Older build available — v3.0.2** | [`KODA-linux-x64.tar.gz`](https://github.com/affinifyhome-lab/KODA-Downloads/releases/download/v3.0.2/KODA-linux-x64.tar.gz) | ~114 MiB |
| **macOS** | ⛔ **No installer published** | — | — |

> The latest release is v3.0.4 and contains Windows only. The Linux archive linked above is from v3.0.2; no macOS installer is available yet. See [Releases](../../releases) for the source of truth.

---

## Windows (beta)

1. Download **`KODA-win-x64.exe`** (~127 MB / ~121 MiB). If the file is ~10 MB, delete it and download again.
2. Wait until the download reaches **100%**.
3. Run the installer from **File Explorer** — do not use **Open** from the browser download bar.
4. If Windows SmartScreen appears, choose **More info → Run anyway**. This build is not Authenticode-signed yet (beta).

After install, KODA opens the desktop setup at `https://kodahub.space/codex/setup`. A valid session continues to the workspace.

---

## Linux (older v3.0.2 archive)

1. Download [`KODA-linux-x64.tar.gz` from v3.0.2](https://github.com/affinifyhome-lab/KODA-Downloads/releases/download/v3.0.2/KODA-linux-x64.tar.gz).
2. Extract it: `tar -xzf KODA-linux-x64.tar.gz`.
3. Launch the extracted app: `chmod +x KODA-linux-x64/devpe-platform && ./KODA-linux-x64/devpe-platform`.

This is an older build, not the current v3.0.4 release. A current Linux AppImage has not been published.

## macOS

There is no macOS `.dmg` in the published releases yet, so a macOS desktop download is not available. Check [Releases](../../releases) for updates; do not use unofficial mirrors.

---

## Safety

- **Source of truth:** only files attached to [GitHub Releases](../../releases) in this repo.
- **Open source app:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda)
- **No account required** to download. No payment on this page.

Questions: [kodahub.space](https://kodahub.space) · Affinify

---

# Português

Instaladores públicos oficiais do **KODA Desktop** (shell Electron que abre `https://kodahub.space/codex/setup`).

Este repositório é a **fila de downloads** de todas as plataformas. Instale apenas artefatos publicados na tabela abaixo.

---

## Fila de releases

| Plataforma | Status | Arquivo | Tamanho aprox. |
|------------|--------|---------|----------------|
| **Windows** x64 | ✅ **Beta — disponível** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~127 MB (~121 MiB) |
| **Linux** x64 | ⚠️ **Build antigo disponível — v3.0.2** | [`KODA-linux-x64.tar.gz`](https://github.com/affinifyhome-lab/KODA-Downloads/releases/download/v3.0.2/KODA-linux-x64.tar.gz) | ~114 MiB |
| **macOS** | ⛔ **Nenhum instalador publicado** | — | — |

> A release mais recente é a v3.0.4 e contém apenas Windows. O arquivo Linux acima é da v3.0.2; ainda não há instalador macOS. A página de [Releases](../../releases) é a fonte oficial.

---

## Windows (beta)

1. Baixe **`KODA-win-x64.exe`** (~127 MB / ~121 MiB). Se o arquivo tiver ~10 MB, apague e baixe de novo.
2. Aguarde **100%** do download.
3. Execute pelo **Explorer** — não use **Abrir** na barra de download do navegador.
4. Se o SmartScreen aparecer, escolha **Mais informações → Executar assim mesmo**. Este build ainda não tem assinatura Authenticode (beta).

Após instalar, o KODA abre o setup do Desktop em `https://kodahub.space/codex/setup`. Uma sessão válida segue direto para o workspace.

---

## Linux (arquivo antigo v3.0.2)

1. Baixe [`KODA-linux-x64.tar.gz` da v3.0.2](https://github.com/affinifyhome-lab/KODA-Downloads/releases/download/v3.0.2/KODA-linux-x64.tar.gz).
2. Extraia: `tar -xzf KODA-linux-x64.tar.gz`.
3. Abra o app extraído: `chmod +x KODA-linux-x64/devpe-platform && ./KODA-linux-x64/devpe-platform`.

Este é um build antigo, não a release atual v3.0.4. Um AppImage Linux atual ainda não foi publicado.

## macOS

Ainda não existe `.dmg` para macOS nas releases publicadas, então o download desktop para Mac não está disponível. Consulte [Releases](../../releases) para atualizações; não use espelhos não oficiais.

---

## Segurança

- **Fonte oficial:** apenas arquivos em [GitHub Releases](../../releases) neste repositório.
- **App:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda)
- **Sem conta** para baixar. Sem pagamento nesta página.

Dúvidas: [kodahub.space](https://kodahub.space) · Affinify

---

## Verificação dos downloads publicados

Confira estes pontos antes de divulgar a fila de downloads:

| # | Verificação | Comando / onde |
|---|-------------|----------------|
| 1 | Windows atual publicado | `KODA-win-x64.exe` na release mais recente |
| 2 | Linux legado publicado | `KODA-linux-x64.tar.gz` na release `v3.0.2` |
| 3 | macOS publicado | **Pendente:** não há `.dmg` nas releases |

Não marque uma plataforma como disponível até que seu instalador real apareça como asset em uma release deste repositório.
