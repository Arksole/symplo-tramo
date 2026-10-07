# Symplo Tramo

Simulador de la hoja de calificación del examen práctico de circulación del permiso B de la DGT.

Symplo Tramo permite a un acompañante (profesor, familiar o amigo) puntuar una práctica de conducción como lo haría un examinador: anota las faltas con los códigos oficiales, aplica el baremo de apto o no apto, guarda el recorrido con geolocalización y conserva un historial para ver qué errores se repiten de una práctica a otra.

> **Aviso:** Symplo Tramo es un proyecto personal y no oficial. No está vinculado a la Dirección General de Tráfico ni reproduce la aplicación interna que usan los examinadores. Los códigos y criterios se basan en los Criterios de Calificación publicados por la DGT, resumidos con palabras propias. Ante cualquier duda, prevalece la normativa oficial vigente.

---

## Índice

1. [Funciones](#funciones)
2. [Cómo se usa](#cómo-se-usa)
3. [Baremo de calificación](#baremo-de-calificación)
4. [Apartados y códigos](#apartados-y-códigos)
5. [Geolocalización y mapa](#geolocalización-y-mapa)
6. [Ajustes](#ajustes)
7. [Copias de seguridad y Google Drive](#copias-de-seguridad-y-google-drive)
8. [Privacidad y datos](#privacidad-y-datos)
9. [Instalación en GitHub Pages](#instalación-en-github-pages)
10. [Actualizar la aplicación](#actualizar-la-aplicación)
11. [Detalles técnicos](#detalles-técnicos)
12. [Limitaciones conocidas](#limitaciones-conocidas)
13. [Créditos](#créditos)

---

## Funciones

- **Hoja de calificación completa** para la clase B, organizada en los 15 apartados de la DGT, con buscador por código o palabra clave.
- **Tres niveles de falta** con los colores de la consulta de notas de la DGT: leve (naranja), grave o deficiente (rojo) y eliminatoria (negro). En cada código solo aparecen los niveles que existen para él.
- **Criterios desplegables**: al tocar el nombre de un código se muestran los supuestos de cada nivel y un campo de nota opcional.
- **Puntos a vigilar**: lista de códigos destacados que se alimenta sola con las faltas de cada prueba finalizada. Se puede añadir o quitar cualquier código con el icono del ojo fuera de la prueba.
- **Cronómetro** con el objetivo de 25 minutos de duración del examen real.
- **Recuento en directo** de leves, graves y eliminatorias en la barra inferior, sin mostrar el resultado hasta finalizar.
- **Deshacer y rehacer** cualquier acción simple: anotar o quitar faltas, cambios en los puntos a vigilar y borrados del historial. Finalizar una prueba no se puede deshacer.
- **Resultado** con el mismo formato que la consulta de notas de la DGT: apto o no apto, códigos por nivel y motivo.
- **Geolocalización**: cada falta queda asociada a su posición y el recorrido se dibuja sobre un mapa de calles.
- **Historial** de simulaciones con su hoja de resultado, un resumen de los códigos que más se repiten y borrado individual con confirmación.
- **Ajustes** para personalizar la hoja, la prueba, el mapa y el tema.
- **Copias de seguridad** en archivo, por el menú de compartir del sistema o directamente en Google Drive.
- **Modo claro y oscuro**, automático o fijo.

## Cómo se usa

1. **Antes de empezar**, la hoja muestra los códigos sin botones de puntuación. Puedes repasar los criterios y elegir con el ojo qué códigos quieres tener a mano en *Puntos a vigilar*.
2. **Pulsa Iniciar.** Arranca el cronómetro, se activa la ubicación y aparecen los botones de falta junto a cada código:
   - ⊖ círculo con signo menos: **leve**
   - ⚠ triángulo de peligro: **grave**
   - 🛑 octógono con aspa: **eliminatoria**
3. **Anota las faltas** durante la práctica tocando el botón correspondiente. Si quieres añadir una nota (dónde ocurrió, qué pasó), despliega el código y escríbela antes de pulsar el botón.
4. **Pausa** cuando haga falta con el mismo botón de Iniciar. La prueba sigue abierta mientras está en pausa.
5. **Corrige** con los botones de deshacer y rehacer de la cabecera, o quita una falta desde la pestaña *Resultado*.
6. **Pulsa Finalizar prueba** y confirma. A partir de ese momento la prueba queda cerrada y no se puede editar.
7. **Consulta el resultado** en la pestaña *Resultado*: la hoja de calificación aparece arriba, con el mapa del recorrido, y la lista de faltas debajo.
8. **Revisa la evolución** en *Historial*, donde están todas las pruebas finalizadas y los códigos que más se repiten.

> Recomendación: el acompañante debería puntuar en silencio, sin avisar durante la conducción, para que la práctica refleje las condiciones reales del examen.

## Baremo de calificación

El resultado se calcula con el mismo criterio que el examen oficial. La prueba es **no apta** si se da cualquiera de estas situaciones:

| Situación | Resultado |
|---|---|
| 1 falta eliminatoria | No apto |
| 2 faltas graves (deficientes) | No apto |
| 1 falta grave y 5 leves | No apto |
| 10 faltas leves | No apto |

En cualquier otro caso, la prueba es **apta**.

- **Eliminatoria:** conducta que pone en peligro la seguridad propia o la de otros usuarios, o incumplimiento de una norma que constituye infracción grave o muy grave.
- **Grave (deficiente):** conducta que obstaculiza a otros usuarios, impidiendo o dificultando notablemente su circulación.
- **Leve:** cualquier otro incumplimiento que no encaje en las anteriores.

## Apartados y códigos

| Nº | Apartado | Ejemplos |
|---|---|---|
| 1 | Comprobaciones previas | Revisión del vehículo |
| 2 | Instalación en el vehículo | Asiento, espejos, cinturón |
| 3 | Incorporación a la circulación | Observación, señalización, ejecución |
| 4 | Progresión normal | Carril, separaciones, velocidad, observación del entorno |
| 5 | Desplazamientos laterales | Observación, señalización, ejecución |
| 6 | Adelantamientos | Posición, velocidad, lugar, permitir el adelantamiento |
| 7 | Intersecciones | Observación, señalización, posición, velocidad, detención, reanudación |
| 8 | Cambio de sentido | Observación, señalización, lugar, ejecución |
| 9 | Paradas y estacionamientos | Observación, señalización, lugar, ejecución |
| 10 | Inmovilización y abandono del vehículo | Apagar el motor, abrir la puerta |
| 11 | Obediencia de las señales | Agentes, semáforos, señales verticales, marcas viales |
| 12 | Luces | Cruce, carretera, antiniebla, emergencia |
| 13 | Manejo de mandos | Embrague, freno, acelerador, marchas, volante, coordinación |
| 14 | Otros mandos y accesorios | Limpiaparabrisas, claxon, visibilidad |
| 15 | Durante el desarrollo de la prueba | Accidente, pérdida de dominio, intervención del profesor, bordillo |

Cada código incluye en la aplicación la descripción de los supuestos leve, grave y eliminatorio que le corresponden.

## Geolocalización y mapa

Al pulsar **Iniciar**, la aplicación pide permiso para usar la ubicación del dispositivo. Con el permiso concedido:

- Se registra el recorrido aproximadamente cada 15 metros o cada 20 segundos.
- Cada falta queda guardada con su posición, con un enlace *Ver ubicación* en la lista de faltas.
- En la hoja de resultado aparece un mapa con el trazado, la salida (círculo blanco) y cada falta marcada con su color y su código.
- Por defecto el mapa usa un estilo de conducción (CARTO Positron o Dark Matter según el tema), que muestra calles y carreteras sin comercios, cafeterías ni otros puntos de interés. El estilo se cambia en *Ajustes*.

El indicador de la cabecera muestra el estado: *Ubicación activa* con la precisión en metros, *Buscando ubicación*, *Ubicación bloqueada* o *Ubicación no disponible*.

**Requisitos para que funcione:**

- La página tiene que abrirse desde una dirección **https**, como la de GitHub Pages.
- El navegador debe tener permiso de ubicación. En iPhone: *Ajustes → Privacidad y seguridad → Localización → Safari*, en "Mientras se usa" y con "Ubicación exacta" activada. En Android: *Ajustes → Aplicaciones → Chrome → Permisos → Ubicación*.
- La versión publicada dentro del visor de claude.ai no tiene acceso a la ubicación ni a las teselas del mapa. En ese caso la aplicación funciona igual, pero sin posiciones, y el recorrido se muestra como un trazado simple sin calles.

## Ajustes

| Grupo | Opción | Qué hace |
|---|---|---|
| Hoja | Mostrar puntos a vigilar | Muestra u oculta la lista de códigos destacados |
| Hoja | Añadir faltas a puntos a vigilar | Al finalizar, los códigos cometidos se añaden solos a la lista |
| Hoja | Botones de puntuación grandes | Aumenta el tamaño de los botones leve, grave y eliminatoria |
| Prueba | Duración objetivo | 20, 25, 30 o 35 minutos; el cronómetro se subraya al superarla |
| Prueba | Recuento visible durante la prueba | Oculta el recuento para que el conductor no sepa cuántas faltas lleva |
| Prueba | Confirmar antes de finalizar | Muestra o no el aviso de confirmación |
| Prueba | Vibrar al anotar una falta | Solo en móviles compatibles (no en iPhone) |
| Prueba | Mantener la pantalla encendida | Evita que el móvil se bloquee durante la prueba |
| Ubicación y mapa | Registrar ubicación y recorrido | Activa o desactiva la geolocalización |
| Ubicación y mapa | Precisión del recorrido | Distancia mínima entre puntos: 5, 10, 15 o 30 m |
| Ubicación y mapa | Estilo del mapa | Conducción según el tema, conducción claro u oscuro, carreteras en color o detallado (OpenStreetMap) |
| Ubicación y mapa | Nombres de calles | Muestra u oculta las etiquetas en los estilos de conducción |
| Ubicación y mapa | Grosor del recorrido | Fino, medio o grueso |
| Apariencia | Tema | Según el dispositivo, claro u oscuro |

*Restablecer ajustes* vuelve a los valores por defecto sin tocar los datos.

## Copias de seguridad y Google Drive

En *Ajustes → Copias de seguridad*:

- **Descargar copia:** guarda un archivo `symplo-tramo-AAAA-MM-DD.json` con el historial, la última prueba, los puntos a vigilar y los ajustes.
- **Compartir copia:** abre el menú de compartir del sistema para enviar el archivo a Google Drive, Archivos, correo u otra app. No necesita configuración.
- **Importar copia:** añade las simulaciones del archivo que no estén ya en la app, sin borrar las actuales. La importación se puede deshacer.

### Copia directa en Google Drive

Para que la app guarde y recupere la copia en Drive sin pasar por el menú de compartir, hace falta un *Client ID* de Google. Se configura una sola vez:

1. Entra en [console.cloud.google.com](https://console.cloud.google.com) con tu cuenta de Google y crea un proyecto nuevo (por ejemplo, *Symplo Tramo*).
2. En **APIs y servicios → Biblioteca**, busca **Google Drive API** y pulsa **Habilitar**.
3. En **APIs y servicios → Pantalla de consentimiento de OAuth**, elige **Externo**, rellena el nombre de la app y tu correo, y en **Usuarios de prueba** añade tu propia cuenta de Gmail.
4. En **APIs y servicios → Credenciales**, pulsa **Crear credenciales → ID de cliente de OAuth**, tipo **Aplicación web**.
5. En **Orígenes de JavaScript autorizados** añade la dirección de tu GitHub Pages, sin ruta ni barra final: `https://tu-usuario.github.io`.
6. Pulsa **Crear** y copia el **ID de cliente** (termina en `.apps.googleusercontent.com`).
7. En Symplo Tramo, pégalo en *Ajustes → Google Drive → Client ID de Google*.

A partir de ahí:

- **Hacer copia en Drive** pide permiso la primera vez y crea o actualiza el archivo `symplo-tramo-backup.json` en tu Drive.
- **Restaurar desde Drive** recupera las simulaciones de esa copia que no estén en el móvil.
- **Copia automática al finalizar** sube la copia al terminar cada prueba si la sesión de Google sigue abierta (dura una hora). Si no lo está, la app avisa de que hay una copia pendiente.

La app solo pide el permiso `drive.file`, que le da acceso únicamente a los archivos que ella misma crea, no al resto de tu Drive. Mientras el proyecto de Google esté en modo de prueba, Google mostrará un aviso de app no verificada al conectar; es normal en proyectos personales.

## Privacidad y datos

- **Todos los datos se guardan solo en el navegador del dispositivo** mediante `localStorage`. No se envían faltas, historial ni ubicaciones a ningún servidor.
- El repositorio público solo contiene el código de la aplicación, nunca los datos de quien la usa.
- Las copias en Google Drive solo se suben cuando las pides o activas la copia automática, y van a tu propia cuenta.
- Para mostrar el mapa, el navegador descarga las imágenes de las calles de los servidores de CARTO u OpenStreetMap, según el estilo elegido. Esas peticiones revelan la zona aproximada que se está viendo, como cualquier web con mapas.
- Cada navegador guarda sus datos por separado. El historial de Safari no aparece en Chrome, y en iPhone tampoco se comparte entre Safari y el icono añadido a la pantalla de inicio. Conviene usar siempre la misma vía.
- Borrar los datos de navegación del sitio elimina también el historial de Symplo Tramo.

Claves usadas en `localStorage`:

| Clave | Contenido |
|---|---|
| `dgtsim.current` | Prueba en curso: tiempo, faltas y recorrido |
| `dgtsim.history` | Pruebas finalizadas |
| `dgtsim.last` | Última prueba finalizada, mostrada en *Resultado* |
| `dgtsim.watch` | Códigos marcados como puntos a vigilar |
| `dgtsim.settings` | Ajustes de la aplicación |

## Actualizar la aplicación

1. Entra en el repositorio.
2. Pulsa **Add file → Upload files** y sube la nueva versión de `index.html`, que reemplaza a la anterior.
3. Pulsa **Commit changes**.

GitHub Pages publica el cambio en uno o dos minutos. Si el móvil sigue mostrando la versión antigua, recarga la página o cierra y vuelve a abrir la app. Los datos guardados se conservan entre versiones.

## Detalles técnicos

- **Un único archivo** `index.html` con HTML, CSS y JavaScript sin dependencias de compilación.
- **Mapa:** [Leaflet](https://leafletjs.com) 1.9.4, cargado desde cdnjs, con su hoja de estilos incrustada en el archivo, y teselas de [CARTO](https://carto.com/basemaps) y [OpenStreetMap](https://www.openstreetmap.org).
- **Google Drive:** Google Identity Services para el permiso y la API REST de Drive v3 para subir y descargar la copia.
- **Pantalla encendida:** Screen Wake Lock API, disponible en iPhone desde iOS 16.4 y en Chrome para Android.
- **Tipografía:** [Public Sans](https://fonts.google.com/specimen/Public+Sans), servida por Google Fonts, con fuentes del sistema como respaldo.
- **Ubicación:** API estándar `navigator.geolocation.watchPosition` con alta precisión.
- **Almacenamiento:** `localStorage`, con todas las lecturas y escrituras protegidas para que la aplicación funcione aunque el navegador lo bloquee.
- **Interfaz adaptable** a móvil y escritorio, con modo oscuro automático y respeto a las zonas seguras de las pantallas con muesca.

## Limitaciones conocidas

- No es la aplicación oficial de los examinadores. Reproduce la hoja de calificación y el baremo, pero no su interfaz.
- Los criterios están resumidos a partir de los Criterios de Calificación de la DGT de septiembre de 2019. Si la DGT publica una revisión, algunos supuestos pueden cambiar.
- El apartado 10 (inmovilización y abandono del vehículo) está agrupado en un solo código de forma aproximada.
- La precisión de la ubicación depende del dispositivo y de la cobertura GPS. En calles estrechas o con edificios altos, la posición puede desviarse varios metros.
- El historial no se sincroniza solo entre dispositivos. Para pasarlo a otro móvil, exporta una copia en uno e impórtala en el otro, o usa la copia en Google Drive.
- Las teselas del mapa son imágenes ya dibujadas, así que no se pueden quitar elementos sueltos. Los estilos de conducción ya vienen sin comercios ni puntos de interés.

## Créditos

- Criterios de calificación: Dirección General de Tráfico.
- Mapas: © colaboradores de [OpenStreetMap](https://www.openstreetmap.org/copyright), bajo licencia ODbL. Estilos de conducción © [CARTO](https://carto.com/attributions).
- Biblioteca de mapas: [Leaflet](https://leafletjs.com), licencia BSD-2-Clause.
- Tipografía: Public Sans, licencia SIL Open Font License.