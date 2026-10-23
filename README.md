# Impara Academy — App Android

App nativa (Kotlin + Jetpack Compose, Material Design 3) conectada a **impara-academy.com.mx**.

## Qué hace

- **Inicio**: saludo, buscador, "Continúa aprendiendo", diplomados/paquetes, categorías y cursos nuevos.
- **Explorar**: búsqueda en vivo y filtros por categoría, con carga infinita.
- **Curso**: temario, lo que aprenderás, precio/oferta, avance del alumno y botón *Comprar* o *Continuar curso*.
- **Paquete**: cursos incluidos, ahorro y compra del paquete completo.
- **Mis cursos**: cursos del alumno con su avance (En curso / Completados).
- **Perfil**: cuenta, compras, notificaciones, soporte por WhatsApp y cerrar sesión.
- **Iniciar sesión / Crear cuenta** nativos (misma cuenta que el sitio).
- **Pago y lecciones**: se abren dentro de la app con la sesión ya iniciada (enlace de un solo uso).
- **Notificaciones**: la app revisa cada hora los avisos que publiques en *wp-admin → Avisos app*.

## Conexión con WordPress

La app usa la API `wp-json/impara/v1/app/*` que vive en el tema (`inc/md-app-api.php`).

## Compilar

GitHub Actions compila el APK en cada cambio a `main` (pestaña **Actions** / **Releases**).
Localmente: abrir la carpeta en Android Studio y usar *Build → Build APK(s)*.

> El APK de prueba está firmado con `debug.keystore` (incluido). Para publicar en Google Play
> hay que crear una llave de firma propia y generar un AAB.
