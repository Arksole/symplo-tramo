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
6. [Privacidad y datos](#privacidad-y-datos)
7. [Instalación en GitHub Pages](#instalación-en-github-pages)
8. [Actualizar la aplicación](#actualizar-la-aplicación)
9. [Detalles técnicos](#detalles-técnicos)
10. [Limitaciones conocidas](#limitaciones-conocidas)
11. [Créditos](#créditos)

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
- **Modo claro y oscuro** según la configuración del dispositivo.

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
- En la hoja de resultado aparece un mapa de OpenStreetMap con el trazado, la salida (círculo blanco) y cada falta marcada con su color y su código.

El indicador de la cabecera muestra el estado: *Ubicación activa* con la precisión en metros, *Buscando ubicación*, *Ubicación bloqueada* o *Ubicación no disponible*.

**Requisitos para que funcione:**

- La página tiene que abrirse desde una dirección **https**, como la de GitHub Pages.
- El navegador debe tener permiso de ubicación. En iPhone: *Ajustes → Privacidad y seguridad → Localización → Safari*, en "Mientras se usa" y con "Ubicación exacta" activada. En Android: *Ajustes → Aplicaciones → Chrome → Permisos → Ubicación*.
- La versión publicada dentro del visor de claude.ai no tiene acceso a la ubicación ni a las teselas del mapa. En ese caso la aplicación funciona igual, pero sin posiciones, y el recorrido se muestra como un trazado simple sin calles.

## Privacidad y datos

- **Todos los datos se guardan solo en el navegador del dispositivo** mediante `localStorage`. No se envían faltas, historial ni ubicaciones a ningún servidor.
- El repositorio público solo contiene el código de la aplicación, nunca los datos de quien la usa.
- Para mostrar el mapa, el navegador descarga las imágenes de las calles de los servidores de OpenStreetMap. Esas peticiones revelan la zona aproximada que se está viendo, como cualquier web con mapas.
- Cada navegador guarda sus datos por separado. El historial de Safari no aparece en Chrome, y en iPhone tampoco se comparte entre Safari y el icono añadido a la pantalla de inicio. Conviene usar siempre la misma vía.
- Borrar los datos de navegación del sitio elimina también el historial de Symplo Tramo.

Claves usadas en `localStorage`:

| Clave | Contenido |
|---|---|
| `dgtsim.current` | Prueba en curso: tiempo, faltas y recorrido |
| `dgtsim.history` | Pruebas finalizadas |
| `dgtsim.last` | Última prueba finalizada, mostrada en *Resultado* |
| `dgtsim.watch` | Códigos marcados como puntos a vigilar |

## Instalación en GitHub Pages

1. Crea una cuenta en [github.com](https://github.com) si no la tienes.
2. Pulsa **+ → New repository**, ponle un nombre (por ejemplo `symplo-tramo`), márcalo como **Public** y pulsa **Create repository**.
3. Pulsa **Add file → Upload files**, arrastra `index.html` (y este `README.md` si quieres) y pulsa **Commit changes**. El archivo principal tiene que llamarse exactamente `index.html`.
4. Ve a **Settings → Pages**. En *Source* elige **Deploy from a branch**, en *Branch* elige **main** y la carpeta **/ (root)**, y pulsa **Save**.
5. En uno o dos minutos aparecerá la dirección de la aplicación, con la forma:
   `https://tu-usuario.github.io/symplo-tramo/`
6. Ábrela en el móvil y, para usarla como una app, añádela a la pantalla de inicio:
   - **iPhone (Safari):** botón Compartir → *Añadir a pantalla de inicio*.
   - **Android (Chrome):** menú ⋮ → *Añadir a pantalla de inicio*.

## Actualizar la aplicación

1. Entra en el repositorio.
2. Pulsa **Add file → Upload files** y sube la nueva versión de `index.html`, que reemplaza a la anterior.
3. Pulsa **Commit changes**.

GitHub Pages publica el cambio en uno o dos minutos. Si el móvil sigue mostrando la versión antigua, recarga la página o cierra y vuelve a abrir la app. Los datos guardados se conservan entre versiones.

## Detalles técnicos

- **Un único archivo** `index.html` con HTML, CSS y JavaScript sin dependencias de compilación.
- **Mapa:** [Leaflet](https://leafletjs.com) 1.9.4, cargado desde cdnjs, con su hoja de estilos incrustada en el archivo, y teselas de [OpenStreetMap](https://www.openstreetmap.org).
- **Tipografía:** [Public Sans](https://fonts.google.com/specimen/Public+Sans), servida por Google Fonts, con fuentes del sistema como respaldo.
- **Ubicación:** API estándar `navigator.geolocation.watchPosition` con alta precisión.
- **Almacenamiento:** `localStorage`, con todas las lecturas y escrituras protegidas para que la aplicación funcione aunque el navegador lo bloquee.
- **Interfaz adaptable** a móvil y escritorio, con modo oscuro automático y respeto a las zonas seguras de las pantallas con muesca.

## Limitaciones conocidas

- No es la aplicación oficial de los examinadores. Reproduce la hoja de calificación y el baremo, pero no su interfaz.
- Los criterios están resumidos a partir de los Criterios de Calificación de la DGT de septiembre de 2019. Si la DGT publica una revisión, algunos supuestos pueden cambiar.
- El apartado 10 (inmovilización y abandono del vehículo) está agrupado en un solo código de forma aproximada.
- La precisión de la ubicación depende del dispositivo y de la cobertura GPS. En calles estrechas o con edificios altos, la posición puede desviarse varios metros.
- El historial no se sincroniza entre dispositivos. Para pasarlo a otro móvil habría que exportarlo, función que todavía no existe.

## Créditos

- Criterios de calificación: Dirección General de Tráfico.
- Mapas: © colaboradores de [OpenStreetMap](https://www.openstreetmap.org/copyright), bajo licencia ODbL.
- Biblioteca de mapas: [Leaflet](https://leafletjs.com), licencia BSD-2-Clause.
- Tipografía: Public Sans, licencia SIL Open Font License.

Symplo Tramo es un proyecto de Nil Cañellas.
