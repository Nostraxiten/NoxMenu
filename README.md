<div align="center">
 
# NoxMenu
 
*Framework modular de cliente Fabric para Minecraft 1.21.5*
 
[![Java 21](https://img.shields.io/badge/Java-21-orange.svg?style=for-the-badge)](https://openjdk.org/)
[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.5-green.svg?style=for-the-badge)](https://www.minecraft.net/)
[![Fabric](https://img.shields.io/badge/Fabric-Loader-blue.svg?style=for-the-badge)](https://fabricmc.net/)
[![Version](https://img.shields.io/badge/Version-1.8.2-purple.svg?style=for-the-badge)]()
</div>

## Descripción General

**NoxMenu** es un cliente de Minecraft pensado para hacer el juego más cómodo, útil y personalizable. Está en desarrollo, así que algunas opciones pueden cambiar, no aparecer o funcionar de forma distinta según la situación. Si encuentras un error, puedes reportarlo en el repositorio para ayudar a mejorarlo.

La carpeta con el mod listo para usar está en NoxMenuMod.
---

<img width="1644" height="542" alt="image" src="https://github.com/user-attachments/assets/233a4996-b5aa-4301-91d5-9eadc8780565" />

## Características y Arquitectura

- **Menú fácil de usar**: Funciones organizadas en categorías para encontrar todo más rápido.
- **Opciones personalizables**: Puedes activar, desactivar o ajustar muchas funciones a tu gusto.
- **Ajustes guardados**: Tus cambios y teclas asignadas se guardan automáticamente.
- **Diseño cómodo**: El menú está pensado para ser visual y práctico desde el primer uso.
---

## Módulos y Opciones

El menú tiene muchas funciones organizadas por categorías. Aquí tienes una explicación sencilla de lo que hace cada una:

### Combat (Combate)
*Módulos para ayudarte en peleas y en situaciones de combate.*

| Módulo | Descripción sencilla |
|---|---|
| **AntiKnockback** | Reduce el empuje cuando te golpean. |
| **AutoBlock** | Bloquea automáticamente cuando lo necesitas. |
| **AutoTotem** | Usa un tótem de forma automática si te queda poca vida. |
| **BowPredictionAim** | Ayuda a apuntar mejor con el arco. |
| **Criticals** | Hace que tus golpes se sientan más fuertes. |
| **HitboxExpand** | Te ayuda a acertar golpes más fácilmente. |
| **KillAura** | Ataca automáticamente al objetivo cercano. |
| **Reach** | Aumenta el alcance de tus ataques. |
| **SilentAim** | Ayuda a golpear al objetivo sin que la cámara se mueva mucho. |
| **TriggerBot** | Golpea al instante cuando el objetivo está en tu mira. |

### Movement (Movimiento)
*Módulos para moverte mejor y de formas más rápidas.*

| Módulo | Descripción sencilla |
|---|---|
| **AntiVoid** | Te ayuda a evitar caer al vacío. |
| **AutoSprint** | Mantiene el sprint activo mientras te mueves. |
| **Fly** | Te permite volar por el mundo. |
| **FreecamNoclip** | Te deja moverte libremente y atravesar bloques. |
| **Jesus** | Te ayuda a caminar sobre agua o lava. |
| **NoFall** | Evita el daño por caída. |
| **NoSlowdown** | Reduce la lentitud al correr, comer o usar arco. |
| **Speed** | Aumenta tu velocidad de movimiento. |
| **Spider** | Te deja trepar paredes. |
| **Step** | Te ayuda a subir escalones más fácilmente. |

### Player (Jugador)
*Módulos para facilitar la experiencia de juego y la gestión del personaje.*

| Módulo | Descripción sencilla |
|---|---|
| **AntiAFK** | Evita que te saquen por inactividad. |
| **AutoEat** | Come automáticamente cuando necesitas comida. |
| **AutoRespawn** | Te hace reaparecer más rápido al morir. |
| **ChestStealer** | Saca todo de un cofre automáticamente. |
| **HUDOverlay** | Muestra información útil en pantalla como FPS, coordenadas y más. |
| **NotificationSystem** | Muestra avisos visuales sencillos del cliente. |
| **PanicKey** | Desactiva todo de golpe si lo necesitas. |

### Render (Visuales)
*Módulos para cambiar cómo ves el mundo y los objetos.*

| Módulo | Descripción sencilla |
|---|---|
| **BlockESP** | Marca bloques importantes a través de las paredes. |
| **ChestClusters** | Agrupa cofres cercanos y los resalta. |
| **Chams** | Hace que algunas entidades se vean más visibles. |
| **ESP** | Muestra la posición de jugadores o criaturas. |
| **Freecam** | Te permite ver el mundo desde otra cámara. |
| **FullBright** | Ilumina el entorno para ver mejor. |
| **NoFog** | Quita la niebla para ver más lejos. |
| **NoHurtCam** | Elimina el efecto de cámara al recibir daño. |
| **NoParticles** | Quita las partículas para mejorar el rendimiento. |
| **StorageESP** | Resalta cofres, barriles y otros contenedores. |
| **Tracers** | Dibuja líneas hacia jugadores o mobs cercanos. |
| **XRay** | Te deja ver minerales a través de bloques comunes. |
| **Zoom** | Acerca la vista cuando lo necesites. |

### World (Mundo)
*Módulos para automatizar tareas y trabajar más rápido en el mundo.*

| Módulo | Descripción sencilla |
|---|---|
| **AutoFish** | Pesca de forma automática. |
| **AutoMine** | Rompe bloques sin tener que mantener el clic todo el tiempo. |
| **AutoTool** | Cambia a la mejor herramienta automáticamente. |
| **Nuker** | Rompe varios bloques a la vez. |
| **Scaffold** | Coloca bloques debajo de tus pies mientras te mueves. |
| **Timer** | Acelera o ralentiza ciertas acciones del juego. |

### Theme (Temas)
*Opciones para cambiar el aspecto del menú.*

| Módulo | Descripción sencilla |
|---|---|
| **CustomTheme** | Permite cambiar los colores del menú y la interfaz. |

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

## Novedades de la Version 1.8.2

- Solo arregla cosas.
