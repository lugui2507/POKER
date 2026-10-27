# Poker Duel (versión sin contraseña)

## Qué hace
- Texas Hold'em multijugador por navegador.
- Sala privada con código; hasta 6 jugadores.
- Nombre personalizado. Escribir `Lucho` activa la vista de administrador para ver cartas ocultas durante una mano.
- Fichas virtuales solamente, sin depósitos, dinero real ni premios canjeables.

## Ejecutar en tu PC
1. Instala Node.js 18 o posterior desde el sitio oficial de Node.js.
2. Descomprime el ZIP.
3. Abre una terminal en esta carpeta.
4. Ejecuta `npm install`.
5. Ejecuta `npm start`.
6. Abre `http://localhost:3000`.

## Cómo hacer que tu amigo entre por Internet
`localhost` solo funciona en tu propia computadora. Para que tu amigo entre desde otra red:
1. Sube esta carpeta a un servicio de alojamiento de aplicaciones compatible con Node.js y WebSockets.
2. Configura el comando de inicio `npm start`.
3. El servicio te dará una URL pública HTTPS, por ejemplo `https://tu-juego.example` (la URL real la entrega el proveedor).
4. Abre esa URL, crea una sala y comparte el código o el enlace con tu amigo.
5. Tu amigo abre la misma URL, escribe su nombre y el código de la sala.

No hay un enlace público creado automáticamente por descargar el ZIP; el paso de alojamiento es necesario. No inventes ni uses la URL de ejemplo como si fuera real.

## Importante sobre Lucho
Como pediste que no haya contraseña, cualquier jugador que escriba `Lucho` recibe el privilegio de ver cartas ocultas. Por tanto, esto NO confirma que realmente seas tú. Para una mesa privada de confianza puede servir como modo de demostración, pero no es seguro en una sala pública.

## Límites de este prototipo
Primera versión de demostración. La lógica de apuestas está simplificada y necesita pruebas adicionales para casos de all-in, botes laterales, reconexiones y todas las variantes de apuestas. No usar para dinero real.
