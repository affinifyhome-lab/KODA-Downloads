# KODA Desktop Downloads

**English** · [Português](#português)

Official public installers for **KODA Desktop** (Electron shell loading `https://kodahub.space/codex/desktop`).

This repository is the official distribution channel for KODA Desktop. The table separates validated downloads from preview artifacts.

---

## Release queue

| Platform | Status | File | Approx. size |
|----------|--------|------|--------------|
| **Windows** x64 | ✅ **Beta — available** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~107 MB |
| **macOS** universal | 🕐 **Queued** — CI pending | `KODA-mac-universal.dmg` | — |
| **Linux** x64 | 🧪 **Preview** — Ubuntu QA pending | [`KODA-linux-x64.tar.gz`](../../releases/latest/download/KODA-linux-x64.tar.gz) | ~114 MiB |

> **Latest tagged release:** see [Releases](../../releases).

---

## Windows (beta)

1. Download **`KODA-win-x64.exe`** (~107 MB). If the file is ~10 MB, delete it and download again.
2. Wait until the download reaches **100%**.
3. Run the installer from **File Explorer** — do not use **Open** from the browser download bar.
4. If Windows SmartScreen appears, choose **More info → Run anyway**. This build is not Authenticode-signed yet (beta).

After install, KODA opens the Codex desktop welcome at `https://kodahub.space/codex/desktop`.

---

## macOS

The macOS installer is not available yet. It will be listed after the build and installation checks are complete.

## Linux (preview)

The latest release contains `KODA-linux-x64.tar.gz` (~114 MiB). This is a preview archive, not the planned AppImage, and it has not passed a clean Ubuntu installation test. Treat it as unverified; Linux support will be marked available after CI and acceptance checks pass.

---

## Safety

- **Source of truth:** only files attached to [GitHub Releases](../../releases) in this repo.
- **Open source app:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda)
- **No account required** to download. No payment on this page.

Questions: [kodahub.space](https://kodahub.space) · Affinify

---

# Português

Instaladores públicos oficiais do **KODA Desktop** (shell Electron que abre `https://kodahub.space/codex/desktop`).

Este repositório é o canal oficial de distribuição do KODA Desktop. A tabela separa downloads validados de artefatos em prévia.

---

## Fila de releases

| Plataforma | Status | Arquivo | Tamanho aprox. |
|------------|--------|---------|----------------|
| **Windows** x64 | ✅ **Beta — disponível** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~107 MB |
| **macOS** universal | 🕐 **Na fila** — CI pendente | `KODA-mac-universal.dmg` | — |
| **Linux** x64 | 🧪 **Prévia** — QA Ubuntu pendente | [`KODA-linux-x64.tar.gz`](../../releases/latest/download/KODA-linux-x64.tar.gz) | ~114 MiB |

> **Release mais recente:** veja [Releases](../../releases).

---

## Windows (beta)

1. Baixe **`KODA-win-x64.exe`** (~107 MB). Se o arquivo tiver ~10 MB, apague e baixe de novo.
2. Aguarde **100%** do download.
3. Execute pelo **Explorer** — não use **Abrir** na barra de download do navegador.
4. Se o SmartScreen aparecer, escolha **Mais informações → Executar assim mesmo**. Este build ainda não tem assinatura Authenticode (beta).

Após instalar, o KODA abre o welcome do Codex em `https://kodahub.space/codex/desktop`.

---

## macOS

O instalador para macOS ainda não está disponível. Ele será listado depois que o build e os testes de instalação forem concluídos.

## Linux (prévia)

A release mais recente contém `KODA-linux-x64.tar.gz` (~114 MiB). Este é um arquivo de prévia, não o AppImage planejado, e ainda não passou por um teste de instalação em Ubuntu limpo. Considere-o não validado; o Linux será marcado como disponível depois que o CI e os testes de aceite passarem.

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
| 3 | Artefatos nos 3 SOs no release | GitHub → KODA-Downloads → Releases → Windows installer + Linux preview archive; DMG after macOS readiness |
| 4 | README público sincronizado | job `Sync KODA-Downloads README` ou `npm run desktop:sync-readme` (requer `gh auth`) |
| 5 | Ícone no instalador | `electron/icon.png` + `npm run desktop:icon` antes de cada `desktop:pack:*` |

**Bloqueador conhecido:** GitHub Actions billing deve estar ativo antes de publicar tag; resolver em GitHub Settings → Billing (manual).
