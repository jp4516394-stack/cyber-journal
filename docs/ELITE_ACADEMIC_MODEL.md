# Modelo académico de referencia: CyberSegyrudad — JorgeVanne

**Propósito:** diseñar una formación independiente de alta exigencia para Jorge Peña (`rtX3e-18`) y Vannesa Pulido (`swtnnes-22`). Se usan referencias de universidades de investigación; **no** se afirma afiliación, título ni crédito académico.

**Inicio real:** ambos programan, pero están comenzando con Linux y ciberseguridad. Un syllabus universitario avanzado es la **meta de formación**, no el punto de partida inmediato.

**Actualizado:** 2026-10-09. Las plataformas, temarios y accesos pueden cambiar; verificar la versión del curso antes de asignar una actividad.

## A. Universidades y materiales oficiales seleccionados

| Área | Universidad / grupo | Curso o recurso | Uso pedagógico | Prerrequisitos |
| --- | --- | --- | --- | --- |
| Seguridad general | UC Berkeley | [CS161 — Computer Security (texto abierto)](https://textbook.cs161.org/) | Fundamentos de redes, memoria, web y criptografía | Programación, redes introductorias |
| Sistemas seguros | MIT / CSAIL | [6.5660 — Computer Systems Security, 2026](https://css.csail.mit.edu/6.5660/2026/general.html) | Arquitecturas seguras, papers, laboratorios e investigación | Sistemas operativos, redes, programación |
| Web, redes y análisis de fallos | Stanford | [CS155 — Computer and Network Security, Spring 2026](https://cs155.stanford.edu/syllabus.html) | Estudios de caso, modelo web, papers y proyectos prácticos | Redes y sistemas |
| Criptografía matemática y aplicada | Stanford | [CS255 — Introduction to Cryptography, Winter 2025](https://crypto.stanford.edu/~dabo/courses/cs255_winter25/) | Seguridad semántica, firmas, integridad, protocolos y pruebas | Probabilidad, aritmética modular, demostraciones |
| Blockchain y wallets | Stanford | [CS251 — Blockchain Technologies, Fall 2026](https://cs251.stanford.edu/) | Merkle trees, consenso, Ethereum, wallets, smart contracts | Programación y sistemas; CS255 útil |
| Análisis de programas | Carnegie Mellon | [17-355/665/819 Program Analysis, 2025](https://cmu-program-analysis.github.io/2025/syllabus.html) | CFG, dataflow, symbolic execution, Hoare logic, abstract interpretation | Algoritmos, compiladores, lógica |
| Investigación en seguridad | Carnegie Mellon | [CyLab](https://www.cylab.cmu.edu/research/) | Investigación interdisciplinar y diseño de problemas científicos | Avanzado, según tema |
| Seguridad de sistemas y protocolos | ETH Zürich | [Secure & Trustworthy Systems](https://sectrs.ethz.ch/education.html) y [ZISC](https://zisc.ethz.ch/research/) | Protocolos, redes, hardware, sistemas, métodos formales | Sistemas, matemáticas |

### Referentes científicos para estudiar sus trabajos

- **Dan Boneh (Stanford):** criptografía aplicada, firmas, protocolos y tecnologías blockchain. Empezar por el material oficial CS255 y CS251.
- **David Wagner y colaboradores (UC Berkeley):** metodología de seguridad de sistemas y el texto abierto CS161.
- **CyLab (Carnegie Mellon):** tomar grupos y papers en temas de seguridad de sistemas, blockchain, autonomía y privacidad.
- **MIT CSAIL y ETH Zürich:** estudiar grupos, proyectos y papers específicos, no únicamente marcas institucionales.

**Regla:** citar trabajos concretos por autores y fecha. No usar la reputación de la institución como sustituto de evidencia.

## B. Estructura de cada módulo, estilo universidad de investigación

1. **Syllabus mínimo:** objetivos, prerrequisitos, conceptos, vocabulario y alcance.
2. **Lectura 1 (primaria):** RFC, especificación, documentación de implementación o paper original.
3. **Lectura 2 (académica):** libro o sección de curso universitario, si agrega profundidad.
4. **Problem set:** 3–5 preguntas conceptuales o matemáticas; justificar cada conclusión.
5. **Laboratorio:** reproducible, autorizado, con pruebas y observaciones.
6. **Mini informe técnico:** hipótesis, método, resultado, análisis y bibliografía.
7. **Defensa oral simulada:** tres preguntas exigentes; distinguir memoria de comprensión.
8. **Revisión cruzada:** Jorge revisa el trabajo de Vanne y viceversa.
9. **Criterio de avance:** evaluación basada en evidencia, no duración del módulo.

Cuando un módulo sea introductorio (como Linux), reducir la carga a **una lectura primaria y un laboratorio**; conservar las preguntas y la revisión. No convertir cada día en un trabajo de investigación completo.

## C. Estándar para las lecturas

Cada referencia asignada debe identificar: **institución o autor, título exacto, año o versión, capítulo/sección, enlace estable y justificación**. Si la sección no está verificada, no inventarla.

Por cada paper:
- Problema y threat model.
- Hipótesis, método y supuesto crítico.
- Qué demuestran los datos o las pruebas.
- Limitaciones, resultados no demostrados, reproducibilidad.
- Pregunta de continuación posible.

No confundir arXiv/preprint con evaluación por pares. Verificar conferencia, versión y correcciones.

## D. Seminario de investigación y fuentes de papers

Cuando adquieran los prerrequisitos, leer artículos de:
- [IEEE Symposium on Security and Privacy (S&P) — papers 2026](https://sp2026.ieee-security.org/accepted-papers.html)
- [USENIX Security 2026 — proceedings](https://www.usenix.org/conference/usenixsecurity26/technical-sessions)
- [NDSS 2026 — accepted papers](https://www.ndss-symposium.org/ndss2026/accepted-papers/)
- Conferencias de criptografía **CRYPTO/EUROCRYPT**, consultando publicaciones y archivos oficiales de [IACR](https://www.iacr.org/).

Las conferencias son fuentes de investigación, **no certificaciones**. Comenzar por abstracts, introducciones y evaluaciones; avanzar a demostraciones formales según el nivel.

## E. Investigación progresiva (tres escalones)

### 1. Reproducir
Ejecutar un experimento publicado o una herramienta documentada con entorno controlado, medir y contrastar los resultados.

**Ejemplo inicial:** construir dos políticas de autorización para una API propia y demostrar con pruebas cuándo falla una.

### 2. Comparar
Diseñar benchmarks con métricas, controlar variables, analizar falsos positivos, límites y condiciones de validez.

**Ejemplo intermedio:** comparar reglas Semgrep o CodeQL sobre un conjunto de fallos conocidos y analizar su cobertura.

### 3. Proponer
Formular una pregunta abierta y construir un método, prototipo, prueba o evaluación que aporte conocimiento nuevo. No asumir novedad sin una revisión de literatura.

**Ejemplo avanzado:** prototipar un analizador de invariantes de vaults ERC-4626 y compararlo experimentalmente con herramientas existentes.

## F. Formación matemática progresiva

| Módulo | Contenidos | Uso |
| --- | --- | --- |
| Matemática discreta y lógica | Conjuntos, relaciones, inducción, invariantes, lógica proposicional | Corrección y modelado |
| Probabilidad y estadística | Variables aleatorias, distribuciones, estimación, sesgos | Criptografía, evaluación experimental |
| Álgebra lineal y números | Vectores, matrices, aritmética modular, teoría de números | Criptografía, ML |
| Algoritmos y compiladores | CFG, grafos, dataflow, SSA, complejidad | Program analysis |
| Lógica y solvers | Lógica de Hoare, SAT/SMT, interpretación abstracta | Verificación formal |
| Sistemas económicos | Incentivos, juegos, liquidez, riesgo, precisión | Seguridad DeFi |

No adelantar técnicas formales antes de fortalecer las bases matemáticas necesarias.

## G. Destinos profesionales (sin promesas)

- **Security / Research Engineer:** capacidad demostrable de implementar experimentos, sistemas y herramientas de investigación. No presupone doctorado en todos los puestos.
- **Research Scientist:** publicaciones y aportaciones originales; para muchos roles se favorece o exige posgrado, frecuentemente doctorado.
- **Profesor/investigador universitario:** habitualmente doctorado, publicaciones, experiencia docente e independencia científica; requisitos varían por país e institución.

Portafolio, contribuciones open source y proyectos reproducibles apoyan candidaturas; no reemplazan automáticamente títulos o criterios formales de admisión.

## H. Primer módulo que corresponde ahora

**Tema:** terminal, filesystem y SSH en Linux.  
**Fuente primaria:** [OpenSSH manual — ssh(1)](https://man.openbsd.org/ssh) y documentación local `man ssh`.  
**Práctica:** [OverTheWire Bandit](https://overthewire.org/wargames/bandit/), nivel 0, sin publicar credenciales.  
**Pregunta para defensa:** qué es una conexión SSH, cuál es la función del host remoto y qué diferencia existe entre un comando de shell y una conexión de red.  
**Entregable:** una nota Markdown individual con comandos utilizados, explicación conceptual y referencia verificable.

**Próximo nivel:** Berkeley CS161 como texto transversal. La lectura avanzada de Stanford/MIT/CMU se introduce gradualmente, según prerrequisitos.
