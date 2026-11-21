# Tándem

Consola de escritorio para trabajar con IA (Claude Code y Codex) sobre tus proyectos, en Windows, macOS y Linux.

- Conversa con Claude usando **tu suscripción** (Pro, Max, Team o Enterprise) a través de Claude Code.
- Aprueba cada edición o comando, mira los diffs en vivo y sigue lo que el agente va editando.
- Notas markdown, skills, explorador de archivos y terminal integrada.
- Git completo: ramas, commits, pull/push, historial, resolución de conflictos y pull requests redactados por IA.
- Temas, iconos y barra de estado configurables, con el uso de tu plan y el vencimiento de tu sesión.

Este repositorio solo publica los instaladores.

📖 **[Guía de usuario](https://capl-dev.github.io/tandem-consola-releases/)** (español / English)

## Descargar

Ve a **[Releases](../../releases/latest)** y descarga el archivo de tu sistema:

| Sistema | Archivo |
|---|---|
| Windows 10/11 | `Tandem_x.y.z_x64-setup.exe` (recomendado) o `.msi` |
| macOS con Apple Silicon (M1 o posterior) | `Tandem_x.y.z_aarch64.dmg` |
| macOS con Intel | `Tandem_x.y.z_x64.dmg` |
| Ubuntu / Debian | `.deb` |
| Fedora / RHEL | `.rpm` |
| Cualquier Linux | `.AppImage` |

## Antes de usarla

Tándem usa el Claude Code que tienes instalado, con tu propia sesión:

1. Instala Claude Code (guía oficial: <https://code.claude.com>).
2. Abre una terminal, escribe `claude` e inicia sesión con tu cuenta.
3. Abre Tándem y elige la carpeta de un proyecto.

Si prefieres usar una API key de Anthropic en lugar de la suscripción, cámbialo en **Ajustes → Cuenta**.

## Instalación y avisos del sistema

Los instaladores todavía no están firmados digitalmente, así que el sistema puede advertirte la primera vez:

- **Windows**: si aparece «Windows protegió su PC», pulsa **Más información → Ejecutar de todas formas**. En equipos con *Smart App Control* activado puede bloquearse por completo.
- **macOS**: abre el `.dmg` y arrastra Tándem a Aplicaciones. Si dice que no se puede abrir, haz clic derecho sobre la app → **Abrir**, o ejecuta en la terminal:
  ```bash
  xattr -dr com.apple.quarantine /Applications/Tandem.app
  ```
- **Linux**: `sudo apt install ./Tandem_*.deb` o `sudo dnf install ./Tandem_*.rpm`. Para el AppImage: `chmod +x Tandem_*.AppImage && ./Tandem_*.AppImage`.

Tándem guarda su configuración en `~/.tandem`.

---

<p align="center">Powered by <b>Cristian Pareja</b> · <a href="mailto:Arleypareja4@gmail.com">Arleypareja4@gmail.com</a></p>
