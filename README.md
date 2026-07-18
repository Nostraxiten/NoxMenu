<div align="center">
 
# NoxMenu
 
*Framework modular de cliente Fabric para Minecraft 1.21.5*
 
[![Java 21](https://img.shields.io/badge/Java-21-orange.svg?style=for-the-badge)](https://openjdk.org/)
[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.5-green.svg?style=for-the-badge)](https://www.minecraft.net/)
[![Fabric](https://img.shields.io/badge/Fabric-Loader-blue.svg?style=for-the-badge)](https://fabricmc.net/)
[![Version](https://img.shields.io/badge/Version-1.8.1-purple.svg?style=for-the-badge)]()
</div>

## Descripción General

**NoxMenu** es un cliente en desarollo temprano, es posible que muchas opciones o no aparezcan, no funcionen, o causen crasheos. No es lo esperado bajo las pruebas que realice como autor. Pero es posible bajo circustancias agenas. Cualquier Error encontrado podria reportarse dentro del repositorio para soluciones futuras.
> Hay un pequeño error para el recuadro de la opcion "?". Ignorar si leiste el readme.

La carpeta que contiene el Mod ya exportado a ".jar" es la de NoxMenuMod.
---
 
<img width="1644" height="542" alt="image" src="https://github.com/user-attachments/assets/233a4996-b5aa-4301-91d5-9eadc8780565" />

 
## Características y Arquitectura
 
- **Arquitectura Modular**: Añade o elimina funciones de forma dinámica sin romper el core.
- **EventBus**: Sistema de eventos para comunicar módulos sin acoplamiento.
- **ClickGUI Interactiva**: Interfaz con categorías organizadas, personalizable, arrastrable, con interruptores y deslizadores.
- **Persistencia**: Todos tus ajustes y teclas vinculadas se guardan automáticamente.
- **Mixins Avanzados**: Modificación de mecánicas internas sin tocar el código base del juego.
---
 
## Módulos y Opciones
 
El menú cuenta con una extensa lista de módulos organizados cuidadosamente por categoría. A continuación, se detalla **qué hace exactamente cada opción**:
 
### Combat (Combate)
*Módulos enfocados en la asistencia durante el combate y el daño.*
 
| Módulo | Descripción Exacta |
|---|---|
| **AntiKnockback** | Anula o reduce el retroceso al recibir un golpe, evitando que te empujen o te tiren al vacío. |
| **AutoBlock** | Bloquea ataques automáticamente usando tu espada o escudo justo en el momento exacto de recibir daño. |
| **AutoTotem** | Equipa instantáneamente un Tótem de Inmortalidad en tu mano secundaria de forma automática cuando tu salud es crítica. |
| **BowPredictionAim** | Calcula la caída de la flecha y el movimiento del enemigo, apuntando automáticamente con precisión matemática. |
| **Criticals** | Fuerza un impacto crítico en todos y cada uno de tus ataques modificando tu estado de salto en los paquetes de red. |
| **HitboxExpand** | Expande virtualmente las cajas de colisión (hitboxes) de los enemigos para facilitar enormemente acertar los golpes. |
| **KillAura** | Ataca y golpea automáticamente y a gran velocidad a cualquier entidad o jugador que entre en tu radio de alcance. |
| **Reach** | Aumenta la distancia máxima desde la que puedes interactuar y golpear entidades, otorgándote más alcance. |
| **SilentAim** | Corrige automáticamente tus ataques hacia el enemigo más cercano o vulnerable sin que tu cámara se mueva visualmente. |
| **TriggerBot** | Golpea automáticamente justo en el milisegundo en el que el punto de mira de tu pantalla se cruza con una entidad. |
 
### Movement (Movimiento)
*Módulos para alterar la física y desplazamiento del jugador.*
 
| Módulo | Descripción Exacta |
|---|---|
| **AntiVoid** | Te salva automáticamente de caer al vacío teletransportándote hacia arriba o rebotando para darte la oportunidad de salvarte. |
| **AutoSprint** | Mantiene activado el modo de correr automáticamente siempre que te mueves hacia adelante. |
| **Fly** | Te permite volar libremente por el mundo en modo supervivencia como si estuvieras jugando en modo creativo. |
| **FreecamNoclip** | Variante de vuelo libre que además te permite atravesar directamente cualquier bloque físico del mundo. |
| **Jesus** | Modifica tu física para permitirte caminar o correr por la superficie del agua o lava sin hundirte jamás. |
| **NoFall** | Elimina por completo el daño por caída recibido al saltar o caer desde grandes alturas. |
| **NoSlowdown** | Evita cualquier penalización de movimiento al pasar por telarañas, comer, usar arco o utilizar escudo. |
| **Speed** | Modifica tu fricción y aceleración en el terreno para moverte a velocidades superiores a las del juego base. |
| **Spider** | Te permite trepar cualquier pared vertical de bloques sólidos como si estuvieras subiendo una escalera de mano. |
| **Step** | Aumenta la altura de paso, permitiéndote subir escalones o bloques completos de forma instantánea sin tener que saltar. |
 
### Player (Jugador)
*Mejoras en la interacción y utilidades del propio jugador.*
 
| Módulo | Descripción Exacta |
|---|---|
| **AntiAFK** | Realiza micromovimientos y acciones automáticas programadas para evitar que los servidores te expulsen por inactividad. |
| **AutoEat** | Selecciona la mejor comida de tu inventario y come de manera automática cuando tu nivel de hambre o salud disminuye. |
| **AutoRespawn** | Evita la pantalla de "Has muerto", enviando el paquete de reaparición forzando volver a la vida al instante. |
| **ChestStealer** | Transfiere rápidamente y de forma automática todo el contenido de un cofre a tu inventario nada más abrirlo. |
| **HUDOverlay** | Muestra en pantalla información esencial en tiempo real como coordenadas, FPS, lag (TPS), armadura y módulos activos. |
| **NotificationSystem** | Despliega alertas visuales emergentes, elegantes y no intrusivas en pantalla sobre acciones y eventos del cliente. |
| **PanicKey** | Funciona como un botón de emergencia que desactiva de un solo golpe todos los módulos activos para parecer 100% legítimo. |
 
### Render (Visuales)
*Alteraciones gráficas y mejoras visuales de cómo ves el mundo.*
 
| Módulo | Descripción Exacta |
|---|---|
| **BlockESP** | Resalta bloques de minerales (Diamante, Ancestral, Oro, Hierro, Carbon, Esmeralda, Cobre) a traves de las paredes con lineas de colores especificos y radio configurable. |
| **ChestClusters** | Agrupa cofres, cofres trampa y barriles cercanos usando Union-Find. Dibuja una linea hacia el centroide del grupo, una caja envolvente con margen de un bloque y una etiqueta con el conteo. |
| **Chams** | Modifica el renderizado de las entidades para mostrarlas con un color brillante y sólido totalmente visible tras las paredes. |
| **ESP** | Dibuja cajas 2D/3D (Extra Sensory Perception) precisas alrededor de jugadores y criaturas para revelar sus posiciones fácilmente. |
| **Freecam** | Desprende la cámara de tu cuerpo para explorar los alrededores libremente como espectador, mientras tu personaje físico se queda seguro. |
| **FullBright** | Altera la iluminación interna del juego al infinito permitiendo ver absolutamente todo iluminado, incluso en cuevas oscuras. |
| **NoFog** | Elimina completamente la niebla de la lejanía, del agua profunda y de la lava, mejorando enormemente la visibilidad. |
| **NoHurtCam** | Desactiva el molesto efecto de temblor, inclinación y giro brusco de la cámara que se produce cada vez que recibes daño. |
| **NoParticles** | Elimina por completo todas las partículas del juego, ayudando inmensamente a subir los FPS y mejorar el rendimiento. |
| **StorageESP** | Encuentra y dibuja contornos sobre cajas fuertes, cofres, barriles, hornos y shulkers viéndolos a través del suelo o paredes. |
| **Tracers** | Dibuja finas y precisas líneas de colores desde la cruceta central de tu pantalla directamente hacia los jugadores y mobs cercanos. |
| **XRay** | Hace invisibles todos los bloques comunes sin valor (piedra, tierra, andesita) revelando instantáneamente solo los minerales valiosos. |
| **Zoom** | Acerca la vista de la cámara con una transición fluida y suave, similar al clásico zoom del mod OptiFine pero configurable. |
 
### World (Mundo)
*Automatización y dominio del entorno del juego.*
 
| Módulo | Descripción Exacta |
|---|---|
| **AutoFish** | Detecta el sonido y movimiento del agua cuando un pez muerde el anzuelo, recoge la caña y vuelve a lanzarla sola. |
| **AutoMine** | Mantiene presionado y activo el botón de romper bloques de forma constante para facilitar túneles sin cansarte de presionar el ratón. |
| **AutoTool** | Analiza en microsegundos el bloque que estás mirando y cambia tu mano de forma automática a la mejor herramienta de tu inventario. |
| **Nuker** | Rompe y arrasa al instante con todos los bloques de un área esférica configurada alrededor de ti a una velocidad vertiginosa. |
| **Scaffold** | Coloca mágicamente bloques debajo de tus pies justo a medida que caminas por cornisas o sobre el vacío, tendiendo puentes mientras te mueves. |
| **Timer** | Altera globalmente el Tickrate de tu cliente (acelera o ralentiza) haciendo que corras o realices acciones mucho más rápido que otros jugadores. |

### Theme (Temas)
*Personalizacion visual de la interfaz del cliente.*

| Modulo | Descripcion Exacta |
|---|---|
| **CustomTheme** | Permite cambiar los colores de la interfaz, textos, fondos y degradados de forma interactiva desde el propio juego. |

---
 
## Controles de la Interfaz
 
- **Abrir Menú**: Presiona `Tab + Control` (configurable).
- **Asignar Tecla (Keybind)**: Haz clic derecho en cualquier módulo dentro de la GUI y seguidamente presiona la tecla que desees asignar a ese módulo.
- **Configurar Módulo**: Haz clic en el icono de engranaje o despliega la pestaña de un módulo para ajustar opciones extras precisas (sliders numéricos, opciones de checkbox y menús de modos).
---
 
## Cómo Compilar y Usar
 
Para construir tu propio archivo `.jar` y disfrutar del mod a partir del código fuente:
 
1. **Requisitos**: Java 21 o una versión superior instalada en tu sistema.
2. Abre la terminal o consola de comandos en esta misma carpeta y ejecuta:
   - **En Windows**: `./gradlew.bat build`
   - **En Linux / macOS**: `./gradlew build`
3. Al terminar, el archivo compilado listo para usar aparecerá en la ruta `build/libs/`.
4. Mueve ese archivo `.jar` a tu carpeta local de mods (`%appdata%/.minecraft/mods` en Windows) e inicia el juego asegurándote de usar el perfil cargador de Fabric.
---

> [!WARNING]
> **Descargo de Responsabilidad Educativo**  
> NoxMenu es un proyecto experimental de código abierto. El autor no se responsabiliza de su mal uso en servidores publicos.

## Novedades de la Version 1.8.1

- **Temas Personalizados**: Nueva categoria Theme y modulo CustomTheme para cambiar colores de fondo, degradados y textos del menu directamente en el juego. Se guardan para tu proxima sesion.
- **Selector de Color Avanzado**: Nuevo sistema interactivo con barras de tono, saturacion y brillo para seleccionar de forma sencilla cualquier color sin fallos.
- **Ventanas de Ayuda Centradas**: Los textos de explicacion ahora aparecen siempre fijados en la parte inferior central de la pantalla, evitando tapar el menu sin importar donde hagas clic.
- **Limpieza**: Se elimino NightVision para asegurar que la iluminacion general (FullBright) no tenga conflictos.
