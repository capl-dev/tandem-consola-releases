# Tándem

Consola de escritorio para trabajar con IA (Claude Code y Codex) sobre tus proyectos, en Windows, macOS y Linux.

- Trabaja con **Claude Code** y **Codex** usando tus propias cuentas, y cambia de motor en mitad de una sesión sin perder el hilo.
- Varias cuentas por motor: si una se queda sin tokens, Tándem pasa a la de respaldo y vuelve cuando se restablece el límite.
- Aprueba cada edición o comando, mira los diffs en vivo y sigue lo que el agente va editando.
- Notas markdown, skills, explorador de archivos y terminal integrada.
- Git completo: ramas, commits, pull/push, historial, resolución de conflictos y pull requests redactados por IA.
- Temas, iconos y barra de estado configurables, con el uso de tu plan y el vencimiento de tu sesión.

Este repositorio solo publica los instaladores.

📖 **[Guía de usuario](https://capl-dev.github.io/tandem-consola-releases/)** (español / English) · 🔒 **[Privacidad y seguridad](https://capl-dev.github.io/tandem-consola-releases/privacidad/)**

## Descargar

Ve a **[Releases](../../releases/latest)** y descarga el archivo de tu sistema:

| Sistema | Archivo |
|---|---|
| Windows 10/11 | `Tandem_x.y.z_x64-setup.exe` (recomendado: se instala sin administrador y se actualiza sola) o `.msi` |
| macOS con Apple Silicon (M1 o posterior) | `Tandem_x.y.z_aarch64.dmg` |
| macOS con Intel | `Tandem_x.y.z_x64.dmg` |
| Ubuntu / Debian | `.deb` |
| Fedora / RHEL | `.rpm` |
| Cualquier Linux | `.AppImage` |

## Actualizaciones

Tándem avisa cuando hay una versión nueva y se actualiza desde la propia app con **Actualizar y reiniciar** (también en **Ajustes → Acerca de → Buscar actualizaciones**). Cada actualización va firmada y Tándem verifica la firma antes de instalarla. En Windows esto aplica al instalador `.exe`; si tienes el `.msi`, desinstálalo e instala el `.exe` una vez. La versión de la Microsoft Store se actualiza desde la Store.

## Antes de usarla

Tándem usa los asistentes que tienes instalados, con tu propia sesión. Necesitas al menos uno de los dos; con ambos puedes cambiar de motor y usar uno como respaldo del otro.

### Claude Code

1. Instala Claude Code (guía oficial: <https://code.claude.com>).
2. Abre una terminal, escribe `claude` e inicia sesión con tu cuenta (Pro, Max, Team o Enterprise).

Si prefieres usar una API key de Anthropic en lugar de la suscripción, cámbialo en **Ajustes → Cuenta**.

### Codex

1. Instala Codex (guía oficial: <https://github.com/openai/codex>):
   - **Windows** (PowerShell): `powershell -ExecutionPolicy ByPass -c "irm https://chatgpt.com/codex/install.ps1 | iex"`
   - **macOS / Linux**: `curl -fsSL https://chatgpt.com/codex/install.sh | sh`
   - O con npm en cualquier sistema: `npm install -g @openai/codex`
2. Abre una terminal, escribe `codex` y elige **Sign in with ChatGPT** para iniciar sesión con tu cuenta de ChatGPT. Una cuenta gratuita sirve como respaldo.

### Empezar

1. Abre Tándem. El asistente de bienvenida detecta qué motores tienes y te deja elegir el principal y el de respaldo.
2. Elige la carpeta de un proyecto y escribe lo que necesitas.

Puedes cambiar de motor en cualquier momento desde el selector de la barra superior, y agregar más cuentas en **Ajustes**.

## Instalación y avisos del sistema

Los instaladores todavía no están firmados digitalmente, así que el sistema puede advertirte la primera vez:

- **Windows**: si aparece «Windows protegió su PC», pulsa **Más información → Ejecutar de todas formas**. En equipos con *Smart App Control* activado puede bloquearse por completo.
- **macOS**: abre el `.dmg` y arrastra Tándem a **Aplicaciones**. La primera vez que lo abras, macOS dirá que no puede verificar al desarrollador:
  1. Pulsa **Aceptar** (o **Listo**).
  2. Ve a **Ajustes del Sistema → Privacidad y seguridad** y, abajo, pulsa **Abrir igualmente** junto al aviso de Tándem.
  3. Confirma con tu contraseña. Desde ahí abre normal.

  Alternativa por terminal: `xattr -dr com.apple.quarantine /Applications/Tandem.app`
- **Linux**: `sudo apt install ./Tandem_*.deb` o `sudo dnf install ./Tandem_*.rpm`. Para el AppImage: `chmod +x Tandem_*.AppImage && ./Tandem_*.AppImage`.

Tándem guarda su configuración en `~/.tandem`. No recopila datos sobre ti: consulta la [política de privacidad](https://capl-dev.github.io/tandem-consola-releases/privacidad/).

---

<p align="center">Powered by <b>Cristian Pareja</b> · <a href="mailto:Arleypareja4@gmail.com">Arleypareja4@gmail.com</a> · <a href="https://capl-dev.github.io/tandem-consola-releases/privacidad/">Privacidad</a></p>
