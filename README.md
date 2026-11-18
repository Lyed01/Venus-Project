# Venus Project

Juego de extracción cooperativa en primera persona hecho en Unreal Engine 5.5, solo con Blueprints. Trabajo práctico final de Desarrollo Avanzado de Videojuegos (UADE).

**Integrantes:** Bono Dipacce, Agustin Pereira, Jesus Cergol, Micaela Giordanino.

## De qué trata

La tripulación aterriza en un planeta con una nave destartalada. Hay que extraer el recurso del planeta y defender la nave de unos aliens que rompen sus módulos. Los jugadores deciden cuándo despegar, pero la tormenta llega a un tiempo fijo y, si los alcanza en el planeta, pierden.

- **Planeta 1:** mar de dunas rojizo, con gemas como recurso.
- **Planeta 2:** anillo de hielo nocturno, más exigente.
- **Nave:** hub de dos pisos con Esclusa, Motores, Soporte vital, Extracción, Puente, Armería y Camarotes. Motores, Soporte vital, Extracción y Electricidad tienen un módulo exterior pegado al casco que los aliens pueden atacar.

## Controles

| Acción | Tecla |
|---|---|
| Moverse | WASD |
| Mirar | Mouse |
| Saltar | Espacio |
| Disparar | Clic izquierdo |
| Interactuar y reparar (mantener) | E |
| Pausa | Esc |

## Cómo abrir el proyecto

1. Instalar Unreal Engine 5.5.
2. Clonar el repo (usa Git LFS para los assets binarios) y abrir `Venus001.uproject`.
3. El mapa inicial es `L_Menu` (`Content/Venus/Levels/Menu`). Los niveles jugables son `L_Level01` y `L_Level02`, y la nave está en `Content/Venus/Levels/Ship/L_Ship`.

## Estructura

Todo el contenido está en `Content/Venus/`: `Core` (GameMode, GameState, PlayerController, GameInstance, SaveGame), `Player`, `Weapons`, `Interactables`, `Enemies` (IA con Behavior Tree), `UI`, `VFX` (Niagara), `Audio`, `Data`, `Materials`, `Meshes` y `Levels`.

## Licencias de terceros

Las fuentes (Saira Stencil One y Rajdhani, SIL OFL 1.1) están detalladas en [Licenses/README.md](Licenses/README.md).
