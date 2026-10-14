# Xantolo al Otro Lado

> Videojuego narrativo de realidad virtual en primera persona, desarrollado por Nyx y Regina.

**Xantolo al Otro Lado** es una experiencia narrativa VR de realismo mágico en la que el jugador encarna a Victoria, una joven migrante que participa junto a su familia en Xantolo en Los Ángeles.

Durante el ritual, el alma de su prometido fallecido regresa. A través de exploración, objetos, recuerdos espaciales y acciones rituales, Victoria deberá atravesar el conflicto entre conservar su presencia y permitirle descansar.

El proyecto busca representar el duelo, la memoria, la migración y el ritual mediante interacción física y espacial propia de VR, evitando el combate y priorizando la exploración, la presencia y la narrativa ambiental.

---

## Estado del proyecto

**Fase actual:** preproducción / diseño conceptual.

Actualmente el proyecto se encuentra en definición y prototipado de sus sistemas principales antes de la producción completa.

La primera meta de desarrollo es construir un **vertical slice de aproximadamente 10–15 minutos** que permita validar:

- locomoción y confort en VR;
- interacción con manos y objetos;
- inventario;
- una acción ritual;
- presencia del prometido;
- transición entre cementerio y memoria;
- funcionamiento de un recuerdo jugable;
- rendimiento en Meta Quest 3.

---

## Plataforma y tecnología

| Elemento | Tecnología |
| --- | --- |
| Motor | Unity |
| Plataforma objetivo | Meta Quest 3 standalone |
| Perspectiva | Primera persona |
| Modo | Un jugador |
| Género | Aventura narrativa / experiencia inmersiva VR |
| Dirección visual | Semirrealismo con realismo mágico |
| Duración objetivo | ~2 horas |

> Las versiones específicas de Unity, SDKs y paquetes deberán mantenerse actualizadas en esta sección conforme avance la producción.

---

## Pilares de diseño

### Ritual encarnado

Las acciones rituales se realizan mediante interacción física: observar, encontrar, tomar, inspeccionar, transportar, colocar y seguir señales del entorno.

### Realismo mágico

La memoria y lo espiritual transforman el mundo cotidiano sin separar la experiencia en un “modo fantástico”.

### Memoria espacial

Los recuerdos son espacios jugables que emergen y se mezclan con el cementerio.

### Interacción antes que interfaz

El entorno, el sonido y los personajes comunican información antes que el HUD.

### Duelo sin castigo

No existe combate ni un sistema tradicional de game over. La progresión es principalmente narrativa.

---

## Estructura general

El cementerio funciona como hub principal de la experiencia.

Desde él, el jugador accede progresivamente a recuerdos relacionados con Victoria y su prometido.

Estructura prevista:

1. Cementerio / prólogo
2. Recuerdo — Placita Olvera
3. Cementerio
4. Recuerdo — Santa Monica / Redondo Beach
5. Cementerio
6. Recuerdo — Griffith Observatory
7. Cementerio / ritual final

La estructura continúa sujeta a validación mediante prototipos.

---

## Principios técnicos

El proyecto se diseña para **Meta Quest 3 standalone desde el inicio**.

Las prioridades técnicas incluyen:

- framerate estable;
- baja latencia;
- interacción consistente;
- geometría optimizada;
- LODs para assets escaneados;
- iluminación principalmente baked;
- uso controlado de transparencias, partículas y postprocesado;
- control del número de NPC simultáneos;
- presupuestos de memoria y texturas adecuados para standalone VR.

---

## Estructura del repositorio

La estructura exacta puede cambiar durante preproducción.

```text
Xantolo/
├── Assets/
│   ├── Art/
│   ├── Audio/
│   ├── Materials/
│   ├── Prefabs/
│   ├── Scenes/
│   ├── Scripts/
│   ├── UI/
│   └── Xantolo/
│
├── Packages/
├── ProjectSettings/
│
├── Documentation/
│   ├── Design/
│   ├── Technical/
│   └── Production/
│
├── README.md
├── LICENSE
└── .gitignore
