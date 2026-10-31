# Flujo de solicitud de CV — LANKAMAR
Estado: PREPARADO, NO ACTIVADO (2026-10-31)

La página /solicitar-cv/ recoge email, versión del CV y consentimiento para tramitar una solicitud, a través de FormSubmit, con reCAPTCHA por defecto y correo de aviso al titular. _autoresponse remite al solicitante el enlace correspondiente al PDF elegido. La notificación recibida en Gmail constituye un registro básico; FormSubmit declara retención de 30 días.

## Pasos previos a enlazarla públicamente
1. Probar el formulario con una dirección controlada y activar la dirección destinataria desde el correo de confirmación de FormSubmit.
2. Comprobar recepción tanto en Gmail como en el correo solicitante, con las tres versiones.
3. Verificar cobertura anti-spam, privacidad y política de retención; publicar aviso adecuado.
4. Solo entonces sustituir los botones del CV de portada y /cv por el enlace /solicitar-cv/.

## Límite fundamental
No hay control de acceso real: los tres PDF están en un repositorio público de GitHub Pages, y sus URL seguirán siendo compartibles sin rellenar el formulario. Para exigir registro al acceso, mover los PDF a almacenamiento PRIVADO fuera de GitHub Pages, servirlos por un backend que emita enlaces de corta duración y conserve registro seguro. Después deben eliminarse de la rama pública y evaluarse copias, historial de Git, motores de búsqueda y caches. No se puede revocar un PDF que ya fue obtenido por terceros.

No usar las direcciones del formulario para marketing sin autorización específica. No agregar datos sensibles de solicitantes. Eliminar registros que no se necesiten.
