# KODA Desktop Downloads

**English** · [Português](#português)

Official public installers for **KODA Desktop** (Electron shell loading `https://kodahub.space/codex/setup`).

This repository is the **download queue** for all platforms. Only published artifacts listed below are safe to install.

**Latest release:** [v3.0.2](../../releases/tag/v3.0.2) · [All releases](../../releases)

---

## Release queue

| Platform | Status | File | Approx. size |
|----------|--------|------|--------------|
| **Windows** x64 | ✅ **Beta — available** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~107 MB |
| **Linux** x64 | ✅ **Beta — available** | [`KODA-linux-x64.tar.gz`](../../releases/latest/download/KODA-linux-x64.tar.gz) | ~110 MB |
| **macOS** universal | 🕐 **Build on macOS** | `KODA-mac-universal.dmg` | — |

> Optional Linux **AppImage** (`KODA-linux-x64.AppImage`) ships when built on Linux/macOS or on Windows with **Developer Mode** enabled (symlinks). See [Linux](#linux-beta) below.

---

## Windows (beta)

1. Download **`KODA-win-x64.exe`** (~107 MB). If the file is ~10 MB, delete it and download again.
2. Wait until the download reaches **100%**.
3. Run the installer from **File Explorer** — do not use **Open** from the browser download bar.
4. If Windows SmartScreen appears, choose **More info → Run anyway**. This build is not Authenticode-signed yet (beta).

After install, KODA opens the setup wizard at `https://kodahub.space/codex/setup`.

---

## Linux (beta)

1. Download **`KODA-linux-x64.tar.gz`** from [Latest release](../../releases/latest).
2. Extract: `tar -xzf KODA-linux-x64.tar.gz`
3. Run: `./KODA` (or `./KODA --no-sandbox` if your distro requires it)

**AppImage (optional):** run `npm run desktop:pack:linux:appimage` on Linux, or on Windows after enabling **Settings → System → For developers → Developer Mode**, then `npm run desktop:publish`.

---

## macOS

The **`.dmg`** must be built **on a Mac** (Apple toolchain). From the [Project_Koda](https://github.com/affinifyhome-lab/Project_Koda) repo on macOS:

```bash
npm ci --legacy-peer-deps
npm run desktop:pack:mac
npm run desktop:publish
```

That uploads `KODA-mac-universal.dmg` to this repository (no GitHub Actions billing required).

---

## Publish manually (all platforms)

From **Project_Koda** (private), after building installers into `dist/`:

```bash
npm run desktop:publish      # gh release → affinifyhome-lab/KODA-Downloads
npm run desktop:sync-readme  # sync this README
```

Windows: `npm run desktop:pack:win` · Linux: `npm run desktop:pack:linux:shell` (or full `desktop:pack:linux` on Linux) · macOS: `npm run desktop:pack:mac`

---

## Safety

- **Source of truth:** only files attached to [GitHub Releases](../../releases) in this repo.
- **App source:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda) (private)
- **No account required** to download. No payment on this page.

Questions: [kodahub.space](https://kodahub.space) · Affinify

---

# Português

Instaladores públicos oficiais do **KODA Desktop** (shell Electron que abre `https://kodahub.space/codex/setup`).

Este repositório é a **fila de downloads** de todas as plataformas. Instale apenas artefatos publicados na tabela abaixo.

**Release mais recente:** [v3.0.2](../../releases/tag/v3.0.2) · [Todos os releases](../../releases)

---

## Fila de releases

| Plataforma | Status | Arquivo | Tamanho aprox. |
|------------|--------|---------|----------------|
| **Windows** x64 | ✅ **Beta — disponível** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~107 MB |
| **Linux** x64 | ✅ **Beta — disponível** | [`KODA-linux-x64.tar.gz`](../../releases/latest/download/KODA-linux-x64.tar.gz) | ~110 MB |
| **macOS** universal | 🕐 **Build no macOS** | `KODA-mac-universal.dmg` | — |

> **AppImage** Linux (`KODA-linux-x64.AppImage`) entra no release quando compilado em Linux/macOS ou no Windows com **Modo de desenvolvedor** ativo. Veja [Linux](#linux-beta-1) abaixo.

---

## Windows (beta)

1. Baixe **`KODA-win-x64.exe`** (~107 MB). Se o arquivo tiver ~10 MB, apague e baixe de novo.
2. Aguarde **100%** do download.
3. Execute pelo **Explorer** — não use **Abrir** na barra de download do navegador.
4. Se o SmartScreen aparecer, escolha **Mais informações → Executar assim mesmo**. Este build ainda não tem assinatura Authenticode (beta).

Após instalar, o KODA abre o wizard em `https://kodahub.space/codex/setup`.

---

## Linux (beta)

1. Baixe **`KODA-linux-x64.tar.gz`** no [release latest](../../releases/latest).
2. Extraia: `tar -xzf KODA-linux-x64.tar.gz`
3. Execute: `./KODA` (ou `./KODA --no-sandbox` se a distro exigir)

**AppImage (opcional):** `npm run desktop:pack:linux:appimage` no Linux, ou no Windows com **Configurações → Sistema → Para desenvolvedores → Modo de desenvolvedor**, depois `npm run desktop:publish`.

---

## macOS

O **`.dmg`** só compila **em um Mac**. No repo [Project_Koda](https://github.com/affinifyhome-lab/Project_Koda):

```bash
npm ci --legacy-peer-deps
npm run desktop:pack:mac
npm run desktop:publish
```

Isso publica `KODA-mac-universal.dmg` aqui, **sem** GitHub Actions pago.

---

## Publicar manualmente (todas as plataformas)

No **Project_Koda** (privado), após gerar instaladores em `dist/`:

```bash
npm run desktop:publish
npm run desktop:sync-readme
```

Windows: `npm run desktop:pack:win` · Linux: `npm run desktop:pack:linux:shell` · macOS: `npm run desktop:pack:mac`

---

## Segurança

- **Fonte oficial:** apenas arquivos em [GitHub Releases](../../releases) neste repositório.
- **Código:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda) (privado)
- **Sem conta** para baixar. Sem pagamento nesta página.

Dúvidas: [kodahub.space](https://kodahub.space) · Affinify

---

## Smoke — fila tri-plataforma (QA)

| # | Verificação | Comando / onde |
|---|-------------|----------------|
| 1 | README local com Win / Linux / macOS | `npm test -- tests/unit/docs/koda-downloads-readme.test.ts` |
| 2 | Release notes do template | `docs/Desktop/KODA-Downloads/RELEASE_NOTES.template.md` |
| 3 | Artefatos no release | `KODA-win-x64.exe`, `KODA-linux-x64.tar.gz`, `KODA-mac-universal.dmg` |
| 4 | README público sincronizado | `npm run desktop:sync-readme` |
| 5 | Ícone no instalador | `npm run desktop:icon` antes de cada `desktop:pack:*` |

**Publicação manual (sem Actions):** `npm run desktop:publish` após `desktop:pack:*` em cada SO.
