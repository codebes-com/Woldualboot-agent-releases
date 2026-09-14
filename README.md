# WOL DualBoot Agent

> Wake and control your PC from Android. Official Windows and Linux installers, published by Codebes.
> Enciende y controla tu PC desde Android. Instaladores oficiales para Windows y Linux, publicados por Codebes.

**Language / Idioma:** [English](#english) · [Español](#español)

- ⬇️ **Download / Descargar:** [latest release / última release](https://github.com/codebes-com/woldualboot-agent-releases/releases/latest)
- 🌐 **Website / Web:** [codebes.com](https://codebes.com/en/woldualboot/agent)
- ✉️ **Support / Soporte:** contact@codebes.com

> This repository only holds the installers (`.msi`, `.deb`) and their `SHA256SUMS.txt`. It has no source code and does not accept contributions.
> Este repositorio solo contiene los instaladores (`.msi`, `.deb`) y sus `SHA256SUMS.txt`. No contiene código fuente ni acepta contribuciones.

---

## English

### Install on Windows

1. Download `woldualboot-agent-<version>-windows-amd64.msi` from the [latest release](https://github.com/codebes-com/woldualboot-agent-releases/releases/latest).
2. Double-click the `.msi`.
3. If **"Windows protected your PC"** (SmartScreen) appears, click **"More info" → "Run anyway"**. It shows because the installer is not yet signed with a reputation-backed certificate; only download it from here or from Codebes.
4. Accept the **UAC** prompt (administrator rights are needed for the service and firewall rule).
5. A **service** and the **tray app** are installed. The tray icon appears after you **sign in again**; open it to show the pairing QR.

### Install on Linux (Debian/Ubuntu)

1. Download `woldualboot-agent_<version>_amd64.deb`.
2. Install it from a terminal (resolves the `ethtool` dependency):

   ```bash
   sudo apt install ./woldualboot-agent_<version>_amd64.deb
   ```

   The `./` matters (local file). You can also double-click it; a **"third-party package"** warning is normal in the software centre.
3. The **service starts automatically** (`systemctl status woldualboot-agent` to check). The **tray app** appears at your next graphical sign-in (or run `woldualboot-tray`); open it to show the pairing QR.

Then scan the QR from the Android app. Full guide: [getting started](https://codebes.com/en/documentation/getting-started).

### Verify the download

Compare the downloaded file's SHA-256 with the value in `SHA256SUMS.txt` from the same release.

```powershell
# Windows (PowerShell)
Get-FileHash .\woldualboot-agent-<version>-windows-amd64.msi -Algorithm SHA256
```

```bash
# Linux
sha256sum -c SHA256SUMS.txt --ignore-missing
```

If the value does not match, do not install the file. Full guide: [download verification](https://codebes.com/en/documentation/download-verification).

---

## Español

### Instalar en Windows

1. Descarga `woldualboot-agent-<versión>-windows-amd64.msi` de la [última release](https://github.com/codebes-com/woldualboot-agent-releases/releases/latest).
2. Haz doble clic en el `.msi`.
3. Si aparece **"Windows protegió su PC"** (SmartScreen), pulsa **"Más información" → "Ejecutar de todas formas"**. Sale porque el instalador aún no está firmado con un certificado de reputación; descárgalo solo desde aquí o desde Codebes.
4. Acepta el aviso de **UAC** (hacen falta permisos de administrador para el servicio y el firewall).
5. Se instala un **servicio** y la **aplicación de bandeja**. El icono de la bandeja aparece al **volver a iniciar sesión**; ábrelo para mostrar el QR de emparejamiento.

### Instalar en Linux (Debian/Ubuntu)

1. Descarga `woldualboot-agent_<versión>_amd64.deb`.
2. Instálalo por terminal (resuelve la dependencia `ethtool`):

   ```bash
   sudo apt install ./woldualboot-agent_<versión>_amd64.deb
   ```

   El `./` es importante (archivo local). También puedes hacer doble clic; en el centro de software es normal un aviso de **"paquete de terceros"**.
3. El **servicio arranca solo** (`systemctl status woldualboot-agent` para comprobarlo). La **bandeja** aparece en el siguiente inicio de sesión gráfica (o ejecuta `woldualboot-tray`); ábrela para mostrar el QR.

Después, escanea el QR desde la app Android. Guía completa: [primeros pasos](https://codebes.com/documentacion/primeros-pasos).

### Verificar la descarga

Compara el SHA-256 del archivo descargado con el valor de `SHA256SUMS.txt` de la misma release. Guía completa: [verificación de descargas](https://codebes.com/documentacion/verificacion-descargas).

---

© Codebes · [codebes.com](https://codebes.com)
