# Demo · Actualización anual de datos (Baloto)

Prototipo navegable del flujo de verificación anual de datos: login, home, pop-up de verificación, menú, Mi perfil, cambio de correo y celular con código OTP, y catálogo de avisos.

Es un solo archivo (`index.html`) con todas las imágenes incrustadas. La única dependencia externa es la fuente Montserrat de Google Fonts.

## Publicar en GitHub Pages

1. Crea un repositorio en GitHub (puede ser privado si tu plan permite Pages privadas).
2. Sube el contenido de esta carpeta a la raíz del repositorio: `index.html`, `.nojekyll` y este `README.md`.
3. En el repositorio: **Settings → Pages → Build and deployment**. En *Source* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarda.
4. En uno o dos minutos la demo queda en `https://<usuario>.github.io/<repositorio>/`.

Para probarla en local basta con abrir `index.html` en el navegador.

## Usuarios demo

Todos usan la contraseña `Baloto2026`.

| Documento | Caso |
| --- | --- |
| CC 1152208466 | Datos vencidos: al entrar ve el pop-up |
| CC 52789456 | Datos al día: entra directo al home |
| CC 79456123 | Ya usó sus 5 aplazamientos: el pop-up no tiene X ni "Ahora no" |

El código OTP válido en la demo es `123456`.

## Enlaces por estado (para html.to.design / Figma)

Agrega el estado al final de la URL publicada, por ejemplo `https://<usuario>.github.io/<repositorio>/#perfil`.

| Estado | Enlace |
| --- | --- |
| Iniciar sesión | `#login` |
| Home | `#home` |
| Pop-up abierto | `#popup` |
| Pop-up sin opción de aplazar | `#popup-final` |
| Menú desplegado (móvil) | `#menu` |
| Mi perfil | `#perfil` |
| Cambio de correo | `#correo` |
| Cambio de celular | `#celular` |
| Código OTP correo | `#otp-correo` |
| Código OTP celular | `#otp-celular` |
| Correo actualizado | `#correo-ok` |
| Celular actualizado | `#celular-ok` |
| Catálogo de avisos | `#avisos` |

## Notas

- Los datos viven solo en memoria: recargar la página reinicia la demo.
- Los dos banners del home siguen como espacios reservados (1214×456 px escritorio, 648×456 px móvil).
