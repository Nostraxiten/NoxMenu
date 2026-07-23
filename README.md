<div align="center">
 
# NoxMenu
 
*Framework modular de cliente Fabric para Minecraft 1.21.5*
 
[![Java 21](https://img.shields.io/badge/Java-21-orange.svg?style=for-the-badge)](https://openjdk.org/)
[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.5-green.svg?style=for-the-badge)](https://www.minecraft.net/)
[![Fabric](https://img.shields.io/badge/Fabric-Loader-blue.svg?style=for-the-badge)](https://fabricmc.net/)
[![Version](https://img.shields.io/badge/Version-5.0.0-purple.svg?style=for-the-badge)]()
</div>

## Descripción General

**NoxMenu** es un cliente en desarrollo temprano. Cualquier error encontrado podría reportarse dentro del repositorio para soluciones futuras.

> **Nota importante sobre el Repositorio (GitHub):** 
> Al subirse a GitHub, el código fuente privado (`NoxMenuCode`) no se incluirá en el repositorio remoto. 
> El repositorio solo contendrá las siguientes carpetas:
> - **`NoxMenuMod`**: Contiene la versión principal, estable y funcional (v5.0.0) exportada a `.jar` lista para usar.
> - **`OLDvers`**: Contiene versiones antiguas, experimentales o incompletas. Algunas pueden funcionar pero muchas otras pueden ser inestables, tener funciones rotas o estar desactualizadas. Úsalas con precaución.
---

<img width="1919" height="444" alt="Captura de pantalla 2026-07-22 114545" src="https://github.com/user-attachments/assets/aa63bb2c-6bb8-49f8-858e-7415d2a64212" />

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
| **AutoDodge** | Esquiva automáticamente flechas y proyectiles detectando su trayectoria. |
| **AutoTotem** | Equipa instantáneamente un Tótem de Inmortalidad en tu mano secundaria de forma automática cuando tu salud es crítica. |
| **CrystalAura** | Coloca y explota cristales del end automáticamente para hacer daño de área a tus enemigos. |
| **HitboxExpand** | Expande virtualmente las cajas de colisión (hitboxes) de los enemigos para facilitar enormemente acertar los golpes. |
| **KillAura** | Ataca y golpea automáticamente y a gran velocidad a cualquier entidad o jugador que entre en tu radio de alcance. |
| **KillAuraRealistic** | Variante de KillAura que simula movimientos de cámara humanos y retrasa los ataques para parecer legítimo. |
| **Surround** | Coloca bloques automáticamente a tu alrededor para proteger tus pies de explosiones. |
| **TriggerBot** | Golpea automáticamente justo en el milisegundo en el que el punto de mira de tu pantalla se cruza con una entidad. |
 
### Movement (Movimiento)
*Módulos para alterar la física y desplazamiento del jugador.*
 
| Módulo | Descripción Exacta |
|---|---|
| **AntiVoid** | Te salva automáticamente de caer al vacío teletransportándote hacia arriba o rebotando para darte la oportunidad de salvarte. |
| **AutoSprint** | Mantiene activado el modo de correr automáticamente siempre que te mueves hacia adelante. |
| **Fly** | Te permite volar libremente por el mundo en modo supervivencia como si estuvieras jugando en modo creativo. |
| **Jesus** | Modifica tu física para permitirte caminar o correr por la superficie del agua o lava sin hundirte jamás. |
| **NoclipTP** | Te permite teletransportarte a través de paredes y bloques sólidos de forma segura usando un fallo de desincronización. |
| **NoFall** | Elimina por completo el daño por caída recibido al saltar o caer desde grandes alturas. |
| **Speed** | Modifica tu fricción y aceleración en el terreno para moverte a velocidades superiores a las del juego base. |
| **Spider** | Te permite trepar cualquier pared vertical de bloques sólidos como si estuvieras subiendo una escalera de mano. |
| **Step** | Aumenta la altura de paso, permitiéndote subir escalones o bloques completos de forma instantánea sin tener que saltar. |
 
### Player (Jugador)
*Mejoras en la interacción y utilidades del propio jugador.*
 
| Módulo | Descripción Exacta |
|---|---|
| **AntiAFK** | Realiza micromovimientos y acciones automáticas programadas para evitar que los servidores te expulsen por inactividad. |
| **AutoArmor** | Equipa automáticamente las mejores piezas de armadura que tengas en tu inventario. |
| **AutoEat** | Selecciona la mejor comida de tu inventario y come de manera automática cuando tu nivel de hambre o salud disminuye. |
| **AutoRespawn** | Evita la pantalla de "Has muerto", enviando el paquete de reaparición forzando volver a la vida al instante. |
| **ChestStealer** | Transfiere rápidamente y de forma automática todo el contenido de un cofre a tu inventario nada más abrirlo. |
| **DeathCoords** | Guarda y muestra las coordenadas exactas de tu última muerte en el chat. |
| **HUDOverlay** | Muestra en pantalla información esencial en tiempo real como coordenadas, FPS, lag (TPS), armadura y módulos activos. |
| **NotificationSystem** | Despliega alertas visuales emergentes, elegantes y no intrusivas en pantalla sobre acciones y eventos del cliente. |
| **PanicKey** | Funciona como un botón de emergencia que desactiva de un solo golpe todos los módulos activos para parecer 100% legítimo. |
 
### Render (Visuales)
*Alteraciones gráficas y mejoras visuales de cómo ves el mundo.*
 
| Módulo | Descripción Exacta |
|---|---|
| **BlockESP** | Resalta bloques de minerales (Diamante, Ancestral, Oro, Hierro, Carbon, Esmeralda, Cobre) a traves de las paredes con lineas de colores especificos y radio configurable. |
| **ChestClusters** | Agrupa cofres, cofres trampa y barriles cercanos usando Union-Find. Dibuja una linea hacia el centroide del grupo, una caja envolvente con margen de un bloque y una etiqueta con el conteo. |
| **ESP** | Dibuja cajas 2D/3D (Extra Sensory Perception) precisas alrededor de jugadores y criaturas para revelar sus posiciones fácilmente. |
| **Freecam** | Desprende la cámara de tu cuerpo para explorar los alrededores libremente como espectador, mientras tu personaje físico se queda seguro. |
| **NoFog** | Elimina completamente la niebla de la lejanía, del agua profunda y de la lava, mejorando enormemente la visibilidad. |
| **NoParticles** | Elimina por completo todas las partículas del juego, ayudando inmensamente a subir los FPS y mejorar el rendimiento. |
| **ProjectileTrajectory** | Dibuja una línea que predice exactamente dónde caerán tus flechas o proyectiles antes de lanzarlos. |
| **StorageESP** | Encuentra y dibuja contornos sobre cajas fuertes, cofres, barriles, hornos y shulkers viéndolos a través del suelo o paredes. |
| **Tracers** | Dibuja finas y precisas líneas de colores desde la cruceta central de tu pantalla directamente hacia los jugadores y mobs cercanos. |
| **XRay** | Hace invisibles todos los bloques comunes sin valor revelando instantáneamente solo los minerales valiosos. |
| **Zoom** | Acerca la vista de la cámara con una transición fluida y suave, similar al clásico zoom del mod OptiFine pero configurable. |

### Optimize (Optimización)
*Mejoras de rendimiento y fps para el cliente.*

| Módulo | Descripción Exacta |
|---|---|
| **ChunkOptimizer** | Reduce el lag y stuttering al generar y cargar nuevos chunks limitando la recarga en el motor gráfico. |
| **FPSBoost** | Opciones para desactivar clima, fuego alto, y reducir distancias de dibujado para maximizar fotogramas. |
| **LeavesOptimizer** | Reduce el impacto en la GPU de las hojas de los árboles transformándolas internamente en bloques sólidos (sin transparencia). |
 
### World (Mundo)
*Automatización y dominio del entorno del juego.*
 
| Módulo | Descripción Exacta |
|---|---|
| **AutoFish** | Detecta el sonido y movimiento del agua cuando un pez muerde el anzuelo, recoge la caña y vuelve a lanzarla sola. |
| **AutoMine** | Mantiene presionado y activo el botón de romper bloques de forma constante para facilitar túneles sin cansarte de presionar el ratón. |
| **AutoTool** | Analiza en microsegundos el bloque que estás mirando y cambia tu mano de forma automática a la mejor herramienta de tu inventario. |
| **Scaffold** | Coloca mágicamente bloques debajo de tus pies justo a medida que caminas por cornisas o sobre el vacío, tendiendo puentes mientras te mueves. |
| **VillagerClusters** | Implementa un sistema de clustering para agrupar aldeanos cercanos mostrando métricas precisas. |
| **Chunks** | Chunks visibles diferenciando los de slimes y los normales. |


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
> El autor no se responsabiliza de su mal uso en servidores publicos.

## Novedades de la Version 5.1.0

- **Mejoras al CristalAura** Ahora es mas preciso y mas fluido con ejemplos mejores de su uso y configuraciones.
- **Nuevo Módulo - VillagerClusters (World):** Implementa un sistema para agrupar aldeanos cercanos, mostrando métricas precisas con líneas y cajas envolventes en 3D.
- **Nuevo Módulo - LeavesOptimizer (Optimize):** Reduce el impacto en la GPU de las hojas de los árboles transformándolas internamente en bloques sólidos (sin transparencia) con color verde uniforme configurable, similar al modo "Fast" de Optifine.
- **Fix Crítico X-Ray**: El XRay fue reescrito para no recalcular la malla de colisión de bloques de Minecraft cada tick del juego, lo que resultaba en un grave lag. Ahora funciona como el X-Ray clásico de versiones antiguas (1.8.1). Las telarañas o la arena de almas ya no penalizan la velocidad y están divididos en sus propios toggles.
- **Nuevos Módulos de Optimización (Categoría Optimize)**: Se introducen los módulos `ChunkOptimizer` (estabiliza los fotogramas evitando microtirones al renderizar nuevas áreas de mundo) y `FPSBoost` (elimina renders costosos como la lluvia, animaciones extra o fuego grande).
- **Refactor General**: Optimización general del EventBus interno.

## Al final de esta documentación se adjuntaran capturas de las mejores configuraciones de las herramientas que suelen ser mas usadas.

1. **KillAuraRealistic**
<img width="248" height="366" alt="Captura de pantalla 2026-07-23 113906" src="https://github.com/user-attachments/assets/c63e007b-b4d3-47ad-b194-95c2f8243409" />

2. **Optimizacion y mejoras de vision** 
<img width="526" height="462" alt="Captura de pantalla 2026-07-23 114537" src="https://github.com/user-attachments/assets/081f825c-e296-4b00-94e9-63976da6fa2e" />

3. **CristalAura. Es la mejor versión que pude lograr de esta opcion**
<img width="250" height="606" alt="Captura de pantalla 2026-07-23 142612" src="https://github.com/user-attachments/assets/a8144a49-56a8-451c-abbb-fe9d3117dbc8" />
