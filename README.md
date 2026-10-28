<p align="center">
  <img src="assets/logo.png" alt="La Región Roleplay" width="220"/>
</p>

<h1 align="center"><b>Proximity Chat</b></h1>

<p align="center">Chat de proximidad para roleplay en ER:LC (Roblox). Sin Discord, sin ruido: hablas solo con quien tienes <b>cerca</b> en el juego.</p>

<div align="center">

[![Latest Release][shield-latest]][repo-latest]
[![Downloads][shield-downloads]][repo-latest]
[![Platform Linux][shield-linux]][repo-latest]
[![Platform Windows][shield-windows]][repo-latest]
[![Platform Android][shield-android]][repo-latest]

</div>

<p align="center">
  <a href="https://github.com/AchitoRD/rp-chat-releases/releases/latest">Descargar última versión</a>
</p>

---

## <img src="https://api.iconify.design/material-symbols/chat-rounded.svg?color=%23fb7a05" width="26" height="26" align="absmiddle" alt=""/> Qué es

Un HUD flotante minimalista que vive sobre tu partida: eliges el modo, escribes, y solo lo ven los jugadores cercanos que tengan la app. Los mensajes duran segundos y **nada se guarda**.

- **IC**: hablar en personaje
- **/me**: acción de tu personaje
- **/do**: entorno o resultado
- **OOC**: fuera de rol `(( ... ))`
- **Proximidad real**: si alguien se aleja, el mensaje se vuelve `.....`
- **Overlay flotante** arrastrable en PC, app normal en móvil
- **Auto-actualización** automática (AppImage)

> [!NOTE]
> Proximity Chat **no modifica Roblox ni inyecta nada**. Es una herramienta externa que funciona aparte del juego.

## <img src="https://api.iconify.design/material-symbols/download-rounded.svg?color=%23fb7a05" width="26" height="26" align="absmiddle" alt=""/> Instalación

### <img src="https://api.iconify.design/logos/linux-tux.svg" width="22" height="22" align="absmiddle" alt=""/> Linux (Debian / Ubuntu / Deepin)
```bash
sudo dpkg -i Proximity-Chat_*_amd64.deb
```
O portable, sin instalar:
```bash
chmod +x Proximity-Chat_*_amd64.AppImage
./Proximity-Chat_*_amd64.AppImage
```

### <img src="https://api.iconify.design/logos/microsoft-windows-icon.svg" width="22" height="22" align="absmiddle" alt=""/> Windows
Descarga el `.exe` de la [última release](https://github.com/AchitoRD/rp-chat-releases/releases/latest) y ejecútalo. Si SmartScreen avisa, es por falta de firma: dale a *Más información → Ejecutar de todas formas*.

### <img src="https://api.iconify.design/logos/android-icon.svg" width="22" height="22" align="absmiddle" alt=""/> Android
Descarga el `.apk` de la [última release](https://github.com/AchitoRD/rp-chat-releases/releases/latest) e instálalo.

### <img src="https://api.iconify.design/simple-icons/apple.svg?color=%23fb7a05" width="22" height="22" align="absmiddle" alt=""/> macOS
El `.dmg` está en camino.

## <img src="https://api.iconify.design/material-symbols/sports-esports-rounded.svg?color=%23fb7a05" width="26" height="26" align="absmiddle" alt=""/> Uso

1. Descarga e instala la app.
2. Ábrela e inicia sesión con tu **username de Roblox** (trae tu avatar automáticamente).
3. Entra al private server en Roblox con tus compañeros.
4. Click al logo, elige modo, escribe y presiona Enter. Solo los cercanos lo ven.

> [!IMPORTANT]
> Para que dos personas chateen, **ambas deben estar dentro del juego** (mismo private server) **y** con la app abierta. Fuera del juego el contador marca `0 cerca`.

## <img src="https://api.iconify.design/material-symbols/help-rounded.svg?color=%23fb7a05" width="26" height="26" align="absmiddle" alt=""/> FAQ

<details>
<summary><b>¿Me pueden banear de Roblox?</b></summary>

No. La app no toca el cliente de Roblox: no inyecta, no lee memoria y no automatiza el juego.
</details>

<details>
<summary><b>¿Guardan mis mensajes?</b></summary>

No. Los mensajes viven unos segundos y se borran. Solo se guarda tu avatar y nombre para mostrarte en la lista de jugadores.
</details>

<details>
<summary><b>¿Funciona fuera del juego?</b></summary>

No del todo. Necesitas estar dentro del private server para que la app sepa quién tienes cerca.
</details>

<details>
<summary><b>La app no conecta o dice "server apagado"</b></summary>

Avisa al staff, probablemente el servidor está en mantenimiento.
</details>

## <img src="https://api.iconify.design/material-symbols/description-rounded.svg?color=%23fb7a05" width="26" height="26" align="absmiddle" alt=""/> Licencia

Todos los derechos reservados, La Región Roleplay. La app se distribuye gratis para jugar.

[shield-latest]: https://img.shields.io/github/v/release/AchitoRD/rp-chat-releases?color=fb7a05&label=version
[shield-downloads]: https://img.shields.io/github/downloads/AchitoRD/rp-chat-releases/total?color=fa9418&label=descargas
[shield-linux]: https://img.shields.io/badge/Linux-deb%20%7C%20AppImage-1e0d07?logo=linux&logoColor=white
[shield-windows]: https://img.shields.io/badge/Windows-exe-1e0d07?logo=windows&logoColor=white
[shield-android]: https://img.shields.io/badge/Android-apk-1e0d07?logo=android&logoColor=white
[repo-latest]: https://github.com/AchitoRD/rp-chat-releases/releases/latest
