# Lógica de la Aplicación

## 1. Lógica general

La aplicación se basa en tres elementos principales:

- Lugares.
- Rutas.
- Reportes.

Los usuarios aportan información sobre esos elementos mediante valoraciones, comentarios, fotos y confirmaciones.

## 2. Relación entre datos

- Un usuario puede crear muchas valoraciones.
- Una valoración pertenece a un usuario y a un lugar.
- Un lugar puede tener muchas valoraciones.
- Un lugar puede tener muchas fotos.
- Un usuario puede reportar muchos problemas.
- Un reporte pertenece a una ubicación concreta.
- Una ruta puede estar formada por varios tramos.
- Un tramo puede tener condiciones específicas, como pendiente, escaleras u obstáculos.
- Una alerta SOS pertenece a un usuario y a una ubicación.

## 3. Nivel de accesibilidad de un lugar

El nivel de accesibilidad puede calcularse combinando:

- Respuestas sobre infraestructura.
- Valoraciones de usuarios.
- Confirmaciones recientes.
- Fotos.
- Reportes activos.

Ejemplo de clasificación:

```text
Accesible: cumple la mayoría de condiciones necesarias.
Parcialmente accesible: tiene algunas barreras, pero puede ser usable para ciertos usuarios.
No accesible: presenta barreras importantes.
Sin información suficiente: todavía faltan datos confiables.
```

## 4. Confianza de la información

No toda la información debe tener el mismo peso. La app debería considerar:

- Fecha de la última actualización.
- Cantidad de usuarios que confirmaron el dato.
- Reputación del usuario que aportó la información.
- Evidencia con fotos.
- Coincidencia entre varias reseñas.

Información antigua o no confirmada debe mostrarse con advertencia.

## 5. Lógica de reportes

Estados posibles de un reporte:

```text
Activo
Confirmado
En revisión
Resuelto
Rechazado
Expirado
```

Reglas sugeridas:

- Un reporte nuevo queda como activo.
- Si varios usuarios lo confirman, pasa a confirmado.
- Si varios usuarios indican que ya no existe, pasa a resuelto o expirado.
- Si contiene abuso o información falsa, pasa a rechazado.

## 6. Lógica de rutas

Una ruta accesible no debe calcularse solo por distancia. También debe considerar:

- Escaleras.
- Pendientes.
- Estado de aceras.
- Cruces seguros.
- Obstáculos.
- Iluminación.
- Ascensores o rampas.
- Reportes recientes.
- Preferencias del usuario.

Regla importante: una ruta más larga puede ser mejor si es más accesible.

## 7. Lógica de preferencias

Las preferencias del usuario deben afectar búsquedas y rutas.

Ejemplo:

Si el usuario marca "evitar escaleras", la app debe:

- Ocultar lugares cuya única entrada tenga escaleras.
- Advertir si una ruta incluye escaleras.
- Priorizar alternativas con rampas o ascensores.

## 8. Lógica del botón SOS

El botón SOS debe:

- Estar visible y ser fácil de usar.
- Evitar activaciones accidentales con una confirmación rápida.
- Usar la ubicación actual solo con permiso.
- Enviar mensaje al contacto configurado.
- Mostrar opción de llamada a emergencias.
- Guardar registro de la alerta.

El SOS no debe prometer sustituir servicios oficiales de emergencia. Debe presentarse como una herramienta de aviso y apoyo.

## 9. Moderación

La app debe prevenir:

- Comentarios ofensivos.
- Información falsa.
- Fotos no relacionadas.
- Reportes maliciosos.
- Datos personales expuestos públicamente.

La moderación puede combinar revisión automática, reportes de usuarios y revisión humana.

## 10. Accesibilidad de la propia app

La aplicación también debe ser accesible. Debe seguir principios reconocidos de accesibilidad digital:

- Contenido perceptible.
- Interfaz operable.
- Información comprensible.
- Compatibilidad con tecnologías de asistencia.

Estos principios están alineados con las Pautas de Accesibilidad para el Contenido Web WCAG 2.2 del W3C.

