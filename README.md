# Apps de DanLab · catálogo

Lista de apps que se enseña en el apartado **"Otras apps de DanLab"** dentro de AVRadio, AVLauncher y las demás apps.
Las apps leen `apps.json` al abrir ese apartado: si cambias este archivo, todas ven el cambio sin publicar versiones nuevas.

## Añadir una app

1. Sube su icono (cuadrado, 192×192 px, PNG) a `icons/`.
2. Copia un bloque de `apps.json` y cambia los datos:
   - `device`: `"car"` si es para la pantalla del coche (sale con botón Descargar / Abrir) o `"phone"` si es para el móvil (sale con un código QR para escanear).
   - `package`: el nombre del paquete Android (solo apps del coche; sirve para saber si ya está instalada).
   - `apk`: enlace directo al APK (apps del coche). `url`: página de la app.
   - `qr`: imagen del código QR (apps del móvil), en `qr/`.
   - `desc` y `note`: textos en español (`es`), inglés (`en`) y catalán (`ca`).
3. Comprueba que el archivo sigue siendo válido (comas y llaves) en https://jsonlint.com antes de guardar.

Cada app se salta a sí misma en la lista.
