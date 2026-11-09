"# EL BOSQUE DE LUMINIA  -  Proyecto GDevelop 5 (aventura de fantasía, 2D)"
=====================================================================================

COMO ABRIRLO
1. Instala GDevelop 5 de escritorio (gratis, gdevelop.io) y descomprime esta carpeta completa.
2. En GDevelop: Abrir proyecto > "Abrir un proyecto local" > elige el archivo  game.json
   (deja las carpetas assets/ y audio/ junto a game.json; no las muevas).
3. Pulsa "Previsualizar" (icono de play). El juego parte en la escena Menu.
   Si GDevelop avisa que el proyecto viene de otra version, acepta.

CONTROLES
  Mover: flechas o WASD      Atacar (orbe de luz): ESPACIO      Hablar / abrir: E
  Pedir pista al hada: F     Pausa y controles: P     Avanzar diálogos: E / ENTER / clic

HISTORIA
  Los cristales de luz de Luminia fueron robados por el Golem de la Cueva de Cristal.
  Eres un aprendiz de mago que, junto al hada Lumi, debe recuperarlos.

LAS 13 PANTALLAS (escenas)   [versión 3 - Etapa 1: Nivel 1 ampliado]
  1 Menú            Titulo y controles
  2 Intro           Historia con efecto maquina de escribir
  NIVEL 1 (5 pantallas, se puede volver atrás por los bordes laterales)
  3 Aldea           Anciano (llave), Mira (misión de gemas), cartel, portón
  4 Camino          Tomas (misión de slimes), slimes, cartel
  5 Bosque          Slimes, cofre
  6 Lago            Puente sobre el agua, murciélago, slimes, cofre, cartel
  7 Claro           MINI-JEFE: Rey Slime (embiste y se divide). Suelta un cristal de luz -> portal
  8 Cinemática      TRANSICION entre niveles: VIDEO (video/cinematica.mp4) + animación de respaldo. ENTER la salta
  NIVEL 2
  9 Cueva1          Esqueletos, murciélago, cofre con llave, puerta de piedra
 10 Cueva2          3 cristales (uno en cámara secreta: pisar 3 botones), slimes, esqueletos, murciélagos, portal
 11 Jefe            Golem de Cristal (barra de vida, 2 fases)
 12 Victoria        Final con confeti
 13 GameOver        Reintentar el nivel (ENTER) o volver al menú (M)

MISIONES Y MEJORAS
  - Mira (Aldea): lleva 6 gemas -> Collar de vida (+1 corazón máximo).
  - Tomas (Camino): derrota 4 slimes -> Amuleto veloz (disparas mas rápido).
  - Lo que hiciste ANTES de aceptar una misión también cuenta (gemas que ya llevas, slimes ya derrotados).
    Si ya cumples la meta al hablar con el NPC, te da el premio en el momento.
  - Para agregar misiones: tabla QUESTS en la biblioteca (meta + como se cuenta el progreso).
  - El juego recuerda cofres abiertos, gemas recogidas, puertas abiertas y jefes derrotados al volver a una pantalla.
  - Los carteles ("Sign") cuentan la historia: acércate y pulsa E.

NPCs Y COMPORTAMIENTOS (mínimo pedido: 3)
  - Hada Lumi ......... sigue al avatar con vuelo suave y da pistas (automáticas y con F)
  - Anciano Orin ...... NPC amistoso: dialogo y entrega de la llave (cambia según el progreso)
  - Mira / Tomas ...... NPCs de misión con diálogos que cambian según tu progreso
  - Rey Slime ......... mini-jefe: embiste, se divide en slimes pequeños a media vida y suelta un cristal
  - Slime ............. deambula en su zona y persigue al avatar si se acerca; 2 de vida; puede soltar gemas
  - Esqueleto ......... patrulla una ruta y embiste si el avatar se acerca; 3 de vida
  - Murciélago ........ vuela sobre los obstáculos, se mueve en zigzag y pica contra el avatar; 1 de vida
  - Golem (jefe) ...... persigue y lanza rocas; en la 2a fase es mas rápido y lanza mas
  Avatar frente a ellos: ataque con orbes, dano/invulnerabilidad/retroceso, diálogos, pociones, cofres.
  Avatar frente a objetos: gemas, cristales, pociones, cofres, puertas con llave, portales, colisiones.

SONIDO
  Efectos: pasos, ataque, golpe, daño, muerte, dialogo, gema, cristal, poción, cofre, puerta, portal, rugido,
  victoria y game over. Musica incidental distinta para menú/intro/victoria, aldea, bosque, cinemática, cueva y jefe.

FEEDBACK VISUAL Y EXPERIENCIA DE USUARIO
  Números de daño flotantes, ráfagas de partículas (gemas, cristales, pociones, cofres, enemigos), temblor de
  pantalla (al recibir daño, al golpear al jefe y al abrir puertas), parpadeo de invulnerabilidad, pausa con P
  que muestra los controles, objetivo siempre visible en el HUD y pistas del hada.


