# KODA Desktop Downloads

**English** · [Português](#português)

Official public installers for **KODA Desktop** (Electron app that opens `https://kodahub.space/codex/setup`).

This repository is the download source for all desktop platforms. Use only files attached to a release in this repository.

## Available installers — v3.0.4

| Platform | Status | File | Approx. size |
|----------|--------|------|--------------|
| **Windows** x64 | ✅ **Beta — available** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~127 MB (~121 MiB) |
| **Linux** x64 | ✅ **Available — AppImage** | [`KODA-linux-x64.AppImage`](../../releases/latest/download/KODA-linux-x64.AppImage) | ~144 MB (~137 MiB) |
| **macOS** Intel x64 | ✅ **Available** | [`KODA-mac-x64.dmg`](../../releases/latest/download/KODA-mac-x64.dmg) | ~162 MB (~154 MiB) |
| **macOS** Apple Silicon arm64 | ✅ **Available** | [`KODA-mac-arm64.dmg`](../../releases/latest/download/KODA-mac-arm64.dmg) | ~158 MB (~151 MiB) |

All four installers are attached to the [v3.0.4 release](../../releases/tag/v3.0.4).

## Windows (beta)

1. Download **`KODA-win-x64.exe`**. If the file is only about 10 MB, delete it and download it again.
2. Wait until the download reaches **100%**.
3. Run the installer from **File Explorer** — do not use **Open** from the browser download bar.
4. If Windows SmartScreen appears, choose **More info → Run anyway**. This build is not Authenticode-signed yet.

After installation, KODA opens the desktop setup at `https://kodahub.space/codex/setup`. A valid session continues to the workspace.

## Linux x64 (AppImage)

1. Download [`KODA-linux-x64.AppImage`](../../releases/latest/download/KODA-linux-x64.AppImage).
2. In a terminal, make it executable and launch it:

   ```bash
   chmod +x KODA-linux-x64.AppImage
   ./KODA-linux-x64.AppImage
   ```

## macOS

1. Choose **`KODA-mac-x64.dmg`** for an Intel Mac or **`KODA-mac-arm64.dmg`** for Apple Silicon.
2. Open the `.dmg` and drag KODA to **Applications**.
3. These builds are not signed or notarized yet. If macOS shows a security prompt, confirm that the installer came from this repository's official release before allowing it to open.

## Safety

- **Source of truth:** files attached to [GitHub Releases](../../releases) in this repository.
- **Application source:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda).
- No account or payment is required to download.

Questions: [kodahub.space](https://kodahub.space) · Affinify

---

# Português

Instaladores públicos oficiais do **KODA Desktop** (aplicativo Electron que abre `https://kodahub.space/codex/setup`).

Este repositório é a fonte de download para todas as plataformas desktop. Use apenas arquivos anexados a uma release deste repositório.

## Instaladores disponíveis — v3.0.4

| Plataforma | Status | Arquivo | Tamanho aprox. |
|------------|--------|---------|----------------|
| **Windows** x64 | ✅ **Beta — disponível** | [`KODA-win-x64.exe`](../../releases/latest/download/KODA-win-x64.exe) | ~127 MB (~121 MiB) |
| **Linux** x64 | ✅ **Disponível — AppImage** | [`KODA-linux-x64.AppImage`](../../releases/latest/download/KODA-linux-x64.AppImage) | ~144 MB (~137 MiB) |
| **macOS** Intel x64 | ✅ **Disponível** | [`KODA-mac-x64.dmg`](../../releases/latest/download/KODA-mac-x64.dmg) | ~162 MB (~154 MiB) |
| **macOS** Apple Silicon arm64 | ✅ **Disponível** | [`KODA-mac-arm64.dmg`](../../releases/latest/download/KODA-mac-arm64.dmg) | ~158 MB (~151 MiB) |

Os quatro instaladores estão anexados à [release v3.0.4](../../releases/tag/v3.0.4).

## Windows (beta)

1. Baixe **`KODA-win-x64.exe`**. Se o arquivo tiver apenas cerca de 10 MB, apague e baixe novamente.
2. Aguarde **100%** do download.
3. Execute pelo **Explorador de Arquivos** — não use **Abrir** na barra de downloads do navegador.
4. Se o SmartScreen aparecer, escolha **Mais informações → Executar assim mesmo**. Este build ainda não tem assinatura Authenticode.

Após instalar, o KODA abre o setup do Desktop em `https://kodahub.space/codex/setup`. Uma sessão válida segue direto para o workspace.

## Linux x64 (AppImage)

1. Baixe [`KODA-linux-x64.AppImage`](../../releases/latest/download/KODA-linux-x64.AppImage).
2. No terminal, torne o arquivo executável e abra o app:

   ```bash
   chmod +x KODA-linux-x64.AppImage
   ./KODA-linux-x64.AppImage
   ```

## macOS

1. Escolha **`KODA-mac-x64.dmg`** para Mac Intel ou **`KODA-mac-arm64.dmg`** para Apple Silicon.
2. Abra o `.dmg` e arraste o KODA para **Aplicativos**.
3. Estes builds ainda não têm assinatura nem notarização. Se o macOS mostrar um aviso de segurança, confirme que o instalador veio da release oficial deste repositório antes de permitir a abertura.

## Segurança

- **Fonte oficial:** arquivos anexados às [GitHub Releases](../../releases) deste repositório.
- **Código-fonte do aplicativo:** [affinifyhome-lab/Project_Koda](https://github.com/affinifyhome-lab/Project_Koda).
- Não é necessário criar conta nem pagar para baixar.

Dúvidas: [kodahub.space](https://kodahub.space) · Affinify

## Verification of published downloads

| # | Check | File in release `v3.0.4` |
|---|-------|---------------------------|
| 1 | Windows x64 | `KODA-win-x64.exe` |
| 2 | Linux x64 AppImage | `KODA-linux-x64.AppImage` |
| 3 | macOS Intel x64 | `KODA-mac-x64.dmg` |
| 4 | macOS Apple Silicon arm64 | `KODA-mac-arm64.dmg` |

Do not mark a platform as available until its installer appears as an asset in this repository's release.

## Verificação dos downloads publicados

| # | Verificação | Arquivo na release `v3.0.4` |
|---|-------------|------------------------------|
| 1 | Windows x64 | `KODA-win-x64.exe` |
| 2 | Linux x64 AppImage | `KODA-linux-x64.AppImage` |
| 3 | macOS Intel x64 | `KODA-mac-x64.dmg` |
| 4 | macOS Apple Silicon arm64 | `KODA-mac-arm64.dmg` |

Não marque uma plataforma como disponível até que o instalador correspondente apareça como asset na release deste repositório.
