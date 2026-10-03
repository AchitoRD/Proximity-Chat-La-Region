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
  <a href="https://github.com/AchitoRD/rp-chat-releases/releases/latest">⬇️ Descargar última versión</a>
</p>

---

## Qué es

Un HUD flotante minimalista que vive sobre tu partida: logo → modos **ME / DO / OOC / IC** → escribes → solo lo ven jugadores cercanos con la app. Los mensajes duran segundos y **nada se guarda**.

- 💬 `IC` — hablar en personaje
- 🟠 `/me` — acción de tu personaje
- 🟡 `/do` — entorno / resultado
- ⚪ `OOC` — fuera de rol `(( ... ))`
- 📍 Proximidad real con el mapa de ER:LC (API v2: si se alejan, el mensaje se vuelve `.....`)
- 🪟 Overlay flotante arrastrable en PC · app normal en móvil
- 🔄 Auto-actualización sola (AppImage)

> [!NOTE]
> Proximity Chat **no modifica Roblox ni inyecta nada**. Es una herramienta externa: lee posiciones vía la API privada de tu servidor ER:LC y entrega mensajes por proximidad.

## Instalación

### Linux (Debian / Ubuntu / Deepin)
```bash
sudo dpkg -i Proximity-Chat_*_amd64.deb
```
O portable sin instalar:
```bash
chmod +x Proximity-Chat_*_amd64.AppImage
./Proximity-Chat_*_amd64.AppImage
```

### Windows
Descarga el `.exe` de la [última release](https://github.com/AchitoRD/rp-chat-releases/releases/latest) y ejecútalo. (Si SmartScreen avisa, es por falta de firma: dale a *Más información → Ejecutar de todas formas*.)

### Android
Descarga el `.apk` de la [última release](https://github.com/AchitoRD/rp-chat-releases/releases/latest) e instálalo. Apunta la app a tu servidor (ver [Servidor](#servidor-propio)).

### macOS
`.dmg` en camino. Mientras tanto: usa la versión web contra tu servidor.

## Uso

1. Enciende tu servidor (abajo).
2. Abre la app e inicia sesión con tu **username de Roblox** (trae tu avatar solo).
3. Entra al private server en Roblox con tus compañeros.
4. Click al logo → elige modo → escribe → Enter. Solo los cercanos lo ven.

> [!IMPORTANT]
> Para que dos personas chateen, **ambas deben estar dentro del juego** (mismo private server) **y** con la app abierta. Fuera del juego el contador marca `0 cerca`.

## Servidor propio

¿Quieres correr el backend tú? Está en el [repo privado](https://github.com/AchitoRD/rp-chat) con Docker:

```bash
git clone https://github.com/AchitoRD/rp-chat.git && cd rp-chat
cp server/.env.example server/.env  # rellena JWT_SECRET y ERLC_SERVER_KEY
docker compose up -d --build
```

Necesitas: un VPS barato (Hetzner/Contabo desde ~4€, Oracle siempre gratis) o Railway/Render/Fly.io (con volumen para la DB). GitHub **no** puede hospedar el servidor (solo guarda archivos). Detalles en el README del repo privado.

## FAQ

<details>
<summary><b>¿Me pueden banear de Roblox?</b></summary>

No. La app no toca el cliente de Roblox: no inyecta, no lee memoria, no automatiza el juego. Solo usa APIs públicas (avatar/nombre) y la API privada de **tu propio** servidor ER:LC.
</details>

<details>
<summary><b>¿Guardan mis mensajes?</b></summary>

No. Los mensajes viven segundos en memoria y se borran. La base solo cachea avatar/nombre para el roster.
</details>

<details>
<summary><b>¿Funciona sin el server de ER:LC?</b></summary>

A medias: el chat funciona entre sesiones de la app, pero sin posiciones no hay proximidad real (todo llega como "ubicación desconocida").
</details>

<details>
<summary><b>La app no conecta / dice "server apagado"</b></summary>

Enciende el backend (`docker compose up -d`) y apunta la app a su URL. En móvil usa la IP de tu red u hostname, no `localhost`.
</details>

## Licencia

Todos los derechos reservados — La Región Roleplay. El binario se distribuye gratis para jugar.

[shield-latest]: https://img.shields.io/github/v/release/AchitoRD/rp-chat-releases?color=fb7a05&label=version
[shield-downloads]: https://img.shields.io/github/downloads/AchitoRD/rp-chat-releases/total?color=fa9418&label=descargas
[shield-linux]: https://img.shields.io/badge/Linux-deb%20%7C%20AppImage-1e0d07?logo=linux&logoColor=white
[shield-windows]: https://img.shields.io/badge/Windows-exe-1e0d07?logo=windows&logoColor=white
[shield-android]: https://img.shields.io/badge/Android-apk-1e0d07?logo=android&logoColor=white
[repo-latest]: https://github.com/AchitoRD/rp-chat-releases/releases/latest
