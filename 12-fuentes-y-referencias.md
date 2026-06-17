# Fuentes y Referencias

Esta documentación usa referencias reconocidas para orientar la lógica del producto. No reemplaza una auditoría legal, técnica o de accesibilidad realizada por especialistas.

## Accesibilidad digital

### WCAG 2.2 - W3C

Referencia: [Web Content Accessibility Guidelines 2.2](https://www.w3.org/TR/WCAG22/)

Las WCAG son pautas internacionales para crear contenido digital accesible. Sus principios principales indican que una interfaz debe ser:

- Perceptible.
- Operable.
- Comprensible.
- Robusta.

Aplicación al proyecto:

- La app debe funcionar con lectores de pantalla.
- Los botones deben ser claros y accionables.
- El contraste debe ser suficiente.
- La información no debe depender solo del color.
- El usuario debe poder entender errores, formularios y alertas.

## Accesibilidad física

### ADA Standards for Accessible Design - U.S. Access Board

Referencia: [ADA Standards](https://www.access-board.gov/ada/)

Aunque la normativa exacta puede cambiar según el país, los estándares ADA son una referencia práctica para entender criterios de accesibilidad física, como rutas accesibles, rampas, puertas, baños y señalización.

Aplicación al proyecto:

- La app debe registrar si existen rampas, escalones, ascensores y baños accesibles.
- Debe diferenciar entre accesible y parcialmente accesible.
- Debe permitir fotos y observaciones, porque la accesibilidad real depende del contexto.

## Transporte público

### GTFS Schedule Reference

Referencia: [GTFS Schedule Reference](https://gtfs.org/documentation/schedule/reference/)

GTFS es un estándar usado para publicar datos de transporte público. Incluye campos relacionados con accesibilidad, como accesibilidad para silla de ruedas en paradas, viajes y vehículos cuando el operador proporciona esos datos.

Aplicación al proyecto:

- La app puede usar datos GTFS si una ciudad o empresa de transporte los publica.
- La información comunitaria puede complementar datos oficiales.
- Debe mostrarse si la accesibilidad del transporte está confirmada, no disponible o reportada por usuarios.

## Datos de mapas y accesibilidad comunitaria

### OpenStreetMap Wiki - Wheelchair

Referencia: [OpenStreetMap wheelchair tag](https://wiki.openstreetmap.org/wiki/Key:wheelchair)

OpenStreetMap usa etiquetas comunitarias para indicar si un lugar es accesible para silla de ruedas, parcialmente accesible o no accesible.

Aplicación al proyecto:

- La app puede inspirarse en valores como `yes`, `limited`, `no` y `designated`.
- El modelo de información debe permitir datos parciales.
- La comunidad puede ayudar a mantener información actualizada.

### OpenStreetMap Wiki - Incline

Referencia: [OpenStreetMap incline tag](https://wiki.openstreetmap.org/wiki/Key:incline)

La etiqueta de inclinación ayuda a describir pendientes, un dato importante para rutas accesibles.

Aplicación al proyecto:

- Las rutas deben considerar pendientes y no solo distancia.
- Una pendiente leve, moderada o pronunciada puede cambiar la recomendación para un usuario.

## Privacidad y protección de datos

### Reglamento General de Protección de Datos - Unión Europea

Referencia: [GDPR official legal text](https://eur-lex.europa.eu/eli/reg/2016/679/oj)

El GDPR es una referencia importante sobre protección de datos personales. La app manejaría datos sensibles como ubicación, contactos de emergencia y posibles preferencias relacionadas con discapacidad o salud.

Aplicación al proyecto:

- Pedir consentimiento claro para usar ubicación.
- Explicar qué datos se guardan y para qué.
- Permitir borrar cuenta y datos personales.
- Proteger contactos de emergencia.
- Evitar publicar información privada en reseñas o reportes.

## Recomendaciones funcionales derivadas

- No prometer que una ruta es completamente segura o accesible sin datos suficientes.
- Mostrar fecha de última actualización.
- Diferenciar entre datos oficiales, datos comunitarios y datos sin confirmar.
- Permitir reportar información incorrecta.
- Usar lenguaje claro y no técnico.
- Diseñar la propia app con accesibilidad desde el inicio.

