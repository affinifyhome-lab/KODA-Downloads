# KODA Desktop Downloads

**English** · [Português](#português)

Official public installers for **KODA Desktop** (Electron shell loading `https://kodahub.space/codex/desktop`).

This repository is the **download queue** for all platforms. Only published artifacts listed below are safe to install.

---

## Release queue

| Platform | Status | File | Approx. size |
|----------|--------|------|--------------|
| **Windows** x64 | ✅ **Beta — available** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~107 MB |
| **macOS** universal | 🕐 **Queued** — CI pending | `KODA-mac-universal.dmg` | — |
| **Linux** x64 | 🕐 **Queued** — CI pending | `KODA-linux-x64.AppImage` | — |

> **Latest tagged release:** see [Releases](../../releases).

---

## Windows (beta)

1. Download **`KODA-win-x64.exe`** (~107 MB). If the file is ~10 MB, delete it and download again.
2. Wait until the download reaches **100%**.
3. Run the installer from **File Explorer** — do not use **Open** from the browser download bar.
4. If Windows SmartScreen appears, choose **More info → Run anyway**. This build is not Authenticode-signed yet (beta).

After install, KODA opens the Codex desktop welcome at `https://kodahub.space/codex/desktop`.

---

## macOS & Linux

Installers will appear in this table when the multi-platform CI publishes them. Until then, use the [Releases](../../releases) page to check availability — do not trust unofficial mirrors.

---

## Safety

- **Source of truth:** only files attached to [GitHub Releases](../../releases) in this repo.
- **Open source app:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda)
- **No account required** to download. No payment on this page.

Questions: [kodahub.space](https://kodahub.space) · Affinify

---

# Português

Instaladores públicos oficiais do **KODA Desktop** (shell Electron que abre `https://kodahub.space/codex/desktop`).

Este repositório é a **fila de downloads** de todas as plataformas. Instale apenas artefatos publicados na tabela abaixo.

---

## Fila de releases

| Plataforma | Status | Arquivo | Tamanho aprox. |
|------------|--------|---------|----------------|
| **Windows** x64 | ✅ **Beta — disponível** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~107 MB |
| **macOS** universal | 🕐 **Na fila** — CI pendente | `KODA-mac-universal.dmg` | — |
| **Linux** x64 | 🕐 **Na fila** — CI pendente | `KODA-linux-x64.AppImage` | — |

> **Release mais recente:** veja [Releases](../../releases).

---

## Windows (beta)

1. Baixe **`KODA-win-x64.exe`** (~107 MB). Se o arquivo tiver ~10 MB, apague e baixe de novo.
2. Aguarde **100%** do download.
3. Execute pelo **Explorer** — não use **Abrir** na barra de download do navegador.
4. Se o SmartScreen aparecer, escolha **Mais informações → Executar assim mesmo**. Este build ainda não tem assinatura Authenticode (beta).

Após instalar, o KODA abre o welcome do Codex em `https://kodahub.space/codex/desktop`.

---

## macOS e Linux

Os instaladores entrarão nesta tabela quando o CI multiplataforma publicar. Até lá, consulte [Releases](../../releases) — não use espelhos não oficiais.

---

## Segurança

- **Fonte oficial:** apenas arquivos em [GitHub Releases](../../releases) neste repositório.
- **App:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda)
- **Sem conta** para baixar. Sem pagamento nesta página.

Dúvidas: [kodahub.space](https://kodahub.space) · Affinify

---

## Smoke — fila tri-plataforma (CI / QA)

Checklist rápido após tag `v*.*.*` ou `workflow_dispatch`:

| # | Verificação | Comando / onde |
|---|-------------|----------------|
| 1 | README local tem as 3 linhas da fila (Win / Mac / Linux) | `npm test -- tests/unit/docs/koda-downloads-readme.test.ts` |
| 2 | Release notes geradas do template | job `Generate release notes` em `.github/workflows/desktop-release.yml` |
| 3 | Artefatos nos 3 SOs no release | GitHub → KODA-Downloads → Releases → assets `KODA-win-x64.exe`, `KODA-linux-x64.AppImage`, `KODA-mac-universal.dmg` |
| 4 | README público sincronizado | job `Sync KODA-Downloads README` ou `npm run desktop:sync-readme` (requer `gh auth`) |
| 5 | Ícone no instalador | `electron/icon.png` + `npm run desktop:icon` antes de cada `desktop:pack:*` |

**Bloqueador conhecido:** GitHub Actions billing deve estar ativo antes de publicar tag; resolver em GitHub Settings → Billing (manual).
