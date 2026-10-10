# EMPIECEN AQUÍ — CyberSegyrudad JorgeVanne

> Este archivo es la **puerta de entrada** cada vez que Jorge o Vanne van a estudiar. No comenzar buscando cursos nuevos ni abriendo diez conversaciones.

## ¿Qué documento consulto?

1. **[STUDY_PLAN.md](roadmap/STUDY_PLAN.md)** — syllabus operativo: en qué orden estudiar, objetivos, fuentes, laboratorios y criterios de avance.
2. **[ROADMAP.md](roadmap/ROADMAP.md)** — visión de mediano y largo plazo: AppSec, Web3, matemáticas e investigación.
3. **[PROGRESS.md](roadmap/PROGRESS.md)** — competencias verificadas por persona y cuál es el próximo objetivo.
4. **[ACADEMIC_STANDARD.md](docs/ACADEMIC_STANDARD.md)** — estándares de fuentes, evidencia, informe y evaluación.
5. **[PROJECT_INSTRUCTIONS.md](docs/PROJECT_INSTRUCTIONS.md)** — instrucciones del mentor de ChatGPT.

## Rutina al comenzar cualquier sesión (3 minutos)

1. Revisar **el Issue abierto propio** de la semana en GitHub.
2. Mirar **qué competencia y entregable** están activos en STUDY_PLAN.
3. Abrir la conversación personal (Jorge o Vanne) de ChatGPT y escribir: **«Continuar mi sesión según mi Issue y el syllabus. Soy [Jorge/Vanne]. Empieza revisando el objetivo sin darme la solución.»**
4. Trabajar en **una sola tarea principal**. Si aparece una curiosidad, agregarla al backlog; no cambiar el temario de improviso.

## Rutina de clase de referencia (90–180 minutos)

- 10 min: recuperar conocimientos previos y objetivo.
- 20–35 min: leer la fuente primaria y tomar notas propias.
- 45–100 min: ejecutar laboratorio, experimentar, depurar; si hay atasco, pedir primero una pista conceptual.
- 15–25 min: redactar la evidencia y explicar por qué ocurrió.
- 5 min: registrar lo que falta en el Issue y el próximo paso.

**Si solo disponen de 30 minutos:** lean una sección breve o terminen una prueba; registren dónde parar y no abran un nuevo tema.

## Ritmo semanal sostenible

| Momento | Trabajo |
| --- | --- |
| Inicio de semana (15–20 min) | Seleccionar **una competencia central** y 1–2 entregables; abrir Issue individual. |
| Sesiones de estudio (3–5) | Teoría + práctica sobre el mismo tema. |
| Cierre (30–45 min) | Subir evidencia en rama individual, abrir PR, revisión por la pareja y evaluación del mentor. |
| Tras revisión | Actualizar PROGRESS con enlaces a la evidencia. Si faltan prerrequisitos, repetir práctica, no avanzar por calendario. |

**GitHub es la fuente de verdad** para tareas y evidencia; ChatGPT explica y evalúa, no sustituye registro técnico reproducible.

## Empezar hoy: primera unidad

**Módulo F1.1 — Terminal y SSH, OverTheWire Bandit nivel 0**

- **Antes:** tener terminal Linux, macOS o WSL disponible; si no, la primera tarea es preparar el entorno.
- **Lecturas verificables:** [OpenSSH ssh(1)](https://man.openbsd.org/ssh), [GNU Bash Manual](https://www.gnu.org/software/bash/manual/) y [OverTheWire Bandit](https://overthewire.org/wargames/bandit/).
- **Objetivo:** explicar qué es terminal, shell, host, usuario, puerto y una conexión SSH.
- **Laboratorio:** ingresar al nivel 0 de Bandit siguiendo la consigna oficial, registrar comandos usados **sin publicar contraseñas**.
- **Preguntas de defensa:** ¿qué hace `ssh`? ¿Qué recurso es local y cuál remoto? ¿Cómo distinguir un error de autenticación de uno de conexión?
- **Entregable individual:** nota Markdown breve, explicación propia, enlace a una fuente primaria y un PR con revisión cruzada.

## Convención de nombres sugerida

- Issues: `[Jorge][F1.1] Terminal y SSH`, `[Vanne][F1.1] Terminal y SSH`.
- Branches: `study/jorge-f1-1`, `study/vanne-f1-1`.
- Evidencia individual: `journal/jorge/F1.1-terminal-ssh.md` y `journal/vanne/F1.1-terminal-ssh.md`.

Nadie debe marcar «dominado» un tema sin **explicar, ejecutar, diagnosticar y documentar**, evaluados por separado.

## Regla de protección contra dispersión

**Una unidad activa por persona, una tarea principal por sesión, una revisión semanal.** Bloques avanzados como Solidity, cryptography y AI security permanecen en roadmap, no en la lista diaria, hasta contar con los prerrequisitos.
