# WOL DualBoot Agent: descargas

Instaladores oficiales de **WOL DualBoot Agent**, publicados por Codebes.

- **Descargar la última versión:** [Releases](https://github.com/codebes-com/woldualboot-agent-releases/releases/latest)
- **Web y documentación:** [codebes.com/woldualboot/agent](https://codebes.com/woldualboot/agent)

Este repositorio solo contiene las releases: el instalador `.msi` para Windows, el paquete `.deb` para Debian/Ubuntu y el archivo `SHA256SUMS.txt`. No contiene código fuente ni acepta contribuciones. Para soporte escribe a contact@codebes.com.

## Verificar la descarga

Compara el SHA-256 del archivo descargado con el valor de `SHA256SUMS.txt` de la misma release.

Windows (PowerShell):

```powershell
Get-FileHash .\woldualboot-agent-<version>-windows-amd64.msi -Algorithm SHA256
```

Linux:

```bash
sha256sum -c SHA256SUMS.txt --ignore-missing
```

Si el valor no coincide, no instales el archivo. Guía completa: [verificación de descargas](https://codebes.com/documentacion/verificacion-descargas).

---

## English

Official **WOL DualBoot Agent** installers, published by Codebes.

- **Download the latest version:** [Releases](https://github.com/codebes-com/woldualboot-agent-releases/releases/latest)
- **Website and documentation:** [codebes.com/en/woldualboot/agent](https://codebes.com/en/woldualboot/agent)

This repository only holds releases: the Windows `.msi` installer, the Debian/Ubuntu `.deb` package and `SHA256SUMS.txt`. It contains no source code and does not accept contributions. For support, write to contact@codebes.com.

To verify a download, compare its SHA-256 with the value in `SHA256SUMS.txt` from the same release. Full guide: [download verification](https://codebes.com/en/documentation/download-verification).
