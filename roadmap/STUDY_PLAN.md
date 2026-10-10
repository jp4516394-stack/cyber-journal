# Syllabus operativo — programa autodidacta CyberSegyrudad

**Estudiantes:** Jorge Peña (`rtX3e-18`) y Vannesa Pulido (`swtnnes-22`).  
**Punto de partida:** experiencia como desarrolladores; sin práctica previa acreditada de Linux, redes o seguridad.  
**Objetivo:** adquirir fundamentos, luego auditar aplicaciones web y smart contracts, y progresar hacia ingeniería e investigación.  
**Modelo:** universidad independiente: `lectura → problemas → laboratorio → evidencia → defensa → revisión`.  
**Ritmo inicial sugerido:** 6–10 horas semanales por persona, adaptable. No asumir progreso por transcurso de semanas.

**Cómo usar este documento:** trabajar de arriba abajo y consultar un único **Issue activo por estudiante**; las semanas son orientativas, las evaluaciones mandan.

## I. Secuencia curricular — prerrequisitos y criterios de salida

| Código / bloque | Aprender en orden | Fuentes y práctica principal | Evidencia mínima para avanzar |
| --- | --- | --- | --- |
| **F0. Git + método académico** | Git clone, working tree, staging, commits, ramas, Markdown, referencia bibliográfica | [Pro Git — Getting Started/Git Basics](https://git-scm.com/book/en/v2), guía académica del repositorio | PR individual revisado; citar fuente correctamente |
| **F1. Linux y terminal** | Shell vs kernel, filesystem, rutas, `pwd`, `ls`, `cd`, `cat`, `man`, `find`, `grep`, pipes, permisos, usuarios, procesos, SSH | [GNU Bash Reference Manual](https://www.gnu.org/software/bash/manual/), [OpenSSH manual](https://man.openbsd.org/ssh), [OverTheWire Bandit](https://overthewire.org/wargames/bandit/) | Explicar y ejecutar comandos sin copiarlos, solucionar un error y documentarlo |
| **F2. Redes y protocolo web** | IP, TCP/UDP, puertos, DNS, HTTP, TLS, request/response, cookies, sesiones, SOP/CORS | [MDN — HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP), [RFC 9110 — HTTP Semantics](https://www.rfc-editor.org/rfc/rfc9110), [TryHackMe Pre Security](https://tryhackme.com/path/outline/presecurity) | Capturar y explicar petición HTTP; modelo de red con DNS y TLS |
| **S1. Fundamentos de seguridad** | CIA, trust boundary, least privilege, authentication vs authorization, threat modeling, control de acceso | [UC Berkeley CS161](https://textbook.cs161.org/), [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/) | Threat model de una API propia y pruebas de autorización |
| **W1. Web AppSec básica** | Burp Repeater, SQLi, IDOR, authentication, XSS, CSRF, SSRF; root cause y mitigación | [PortSwigger Academy](https://portswigger.net/web-security), [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/), [OWASP WSTG](https://owasp.org/www-project-web-security-testing-guide/) | Varios labs explicados; un hallazgo web local con prueba y corrección |
| **B1. Ethereum y Solidity** | Hashes, firmas, wallets, cuentas, transacciones, gas, EVM, ABI, `storage`, Solidity, testing | [Ethereum docs](https://ethereum.org/en/developers/docs/), [Solidity docs](https://docs.soliditylang.org/), [Foundry](https://getfoundry.sh/), [Ethernaut](https://ethernaut.openzeppelin.com/) | Contratos simples con tests; explicar control de acceso, cambio de estado y gas |
| **B2. Auditoría Web3** | Reentrancy, oracles, allowances, EIP-712, invariantes, fuzzing, riesgos económicos | [Solidity Security Considerations](https://docs.soliditylang.org/en/latest/security-considerations.html), [Damn Vulnerable DeFi](https://github.com/theredguild/damn-vulnerable-defi) | Auditoría local reproducible y corrección justificada |
| **R. Ingeniería e investigación** | Discreta, lógica, probabilidad, sistemas, compiladores, static analysis, SMT, papers, benchmarking | [CMU Program Analysis](https://cmu-program-analysis.github.io/2025/syllabus.html), [MIT Systems Security](https://css.csail.mit.edu/6.5660/2026/general.html), [Modelo académico](../docs/ELITE_ACADEMIC_MODEL.md) | Reproducir una investigación y analizar resultados/limitaciones |

**Regla para trabajar en paralelo:** solo cuando F1–F2 estén suficientemente comprendidos, introducir microproyectos de Solidity; no intentar AppSec avanzada, EVM y cryptography en la misma semana.

## II. Primer ciclo orientativo — 12 semanas

| Semana | Unidad y pregunta guía | Práctica | Producto semanal |
| --- | --- | --- | --- |
| **1** | **F1.1** ¿Qué es terminal, shell, host remoto y SSH? | Primeros niveles Bandit y comandos Linux básicos; primer PR | Notas individuales + primer PR |
| **2** | **F1.2** ¿Cómo funcionan archivos, permisos y búsqueda? | Bandit guiado, rutas, `file`, `find`, `grep`, `chmod` solo en laboratorio propio | Explicación de permisos y diagnóstico |
| **3** | **F1.3 + F0** ¿Cómo automatizar tareas y colaborar? | Pipes, redirecciones, variables, Git y PR de revisión | Script pequeño + revisión cruzada |
| **4** | **F2.1** ¿Qué son IP, puertos, TCP y DNS? | TryHackMe Pre Security + inspección de conexiones propias | Diagrama de una conexión |
| **5** | **F2.2** ¿Qué ocurre dentro de una petición HTTPS? | HTTP headers, cookies, TLS; DevTools del navegador | Petición HTTP anotada y fuentes |
| **6** | **S1.1** ¿Quién puede hacer qué en una aplicación? | Autenticación vs autorización, roles, API propia | Modelo de amenazas + tests |
| **7** | **W1.1** ¿Cómo observa un auditor una petición? | Burp Proxy/Repeater, scope, laboratorio autorizado | Captura y explicación de petición |
| **8** | **W1.2** ¿Cómo aparece una vulnerabilidad de entrada? | PortSwigger SQLi de nivel introductorio | Causa raíz, prueba y mitigación |
| **9** | **W1.3** ¿Cómo se rompe el control de acceso? | PortSwigger Access Control e IDOR de laboratorio | Test de usuarios y permisos |
| **10** | **W1.4** ¿Qué implica ejecutar contenido no confiable? | PortSwigger XSS introductorio | Comparativa vulnerabilidad/corrección |
| **11** | **W1.5 + B1 orientación** ¿Qué cambia con una aplicación en blockchain? | OWASP Juice Shop; lectura Ethereum Accounts; Remix opcional | Informe web + glosario EVM |
| **12** | **Cierre del primer ciclo** ¿Qué entendemos realmente? | Defensa oral simulada, revisión conjunta y plan siguiente | Evaluación individual y priorización posterior |

**Estas semanas no garantizan dominio**. Una unidad puede tomar varias semanas según errores, disponibilidad y capacidad para explicarla. Solidity/Foundry se amplían en el **siguiente ciclo** cuando F1–F2 y W1 inicial estén sólidas; en personas avanzando más rápido puede introducirse antes con criterio pedagógico.

## III. Primera semana — orden de sesiones

| Sesión | Lectura y teoría | Ejercicio | Criterio observable |
| --- | --- | --- | --- |
| **1 — Inicio** | Conceptos de terminal, shell, SSH y cliente/servidor; fuente OpenSSH | Configurar terminal si falta y conectar a Bandit nivel 0 | Explicar conexión remota sin copiar definiciones |
| **2 — Navegación** | Bash: comandos, rutas, `pwd`, `ls`, `cd` | Experimentar con directorios propios | Distinguir ruta absoluta y relativa |
| **3 — Archivos** | `cat`, `file`, `man`; opción vs argumento | Resolver siguiente nivel Bandit si el anterior fue comprendido | Describir comandos y diagnosticar error |
| **4 — Investigar** | Ayuda local, manuales, `--help` | Resolver un ejercicio sin tutorial completo | Justificar estrategia y fuentes |
| **5 — Git básico** | Clonar, status, branch, add, commit | Crear una nota en rama individual | Commit propio identificable |
| **6 — Documentación** | [Estándar académico](../docs/ACADEMIC_STANDARD.md) | Completar notas y abrir PR | Nota reproducible sin credenciales |
| **7 — Evaluación** | Repaso y preguntas de defensa | Revisión cruzada con la pareja | Evaluación individual y próximo Issue |

La unidad **F1.1** debe completarse antes de acelerar Bandit. Los niveles no se cuentan como experiencia profesional.

## IV. Estructura de cada Issue semanal (copiar)

```markdown
## Estudiante y unidad
- Nombre:
- Código del módulo:
- Estado: En aprendizaje

## Objetivo de la semana
[Una competencia concreta]

## Fuentes obligatorias
- [Autor / título / sección / URL]

## Práctica
- [ ] Lectura primaria y tres preguntas
- [ ] Laboratorio reproducible
- [ ] Explicación propia del mecanismo
- [ ] Documento Markdown / pruebas
- [ ] PR y revisión cruzada

## Evidencia
- Commits/PR:
- Salidas y pruebas (sin secretos):
- Errores encontrados:

## Defensa
1. ¿Por qué funciona?
2. ¿Qué limitaciones tiene?
3. ¿Cómo lo comprobaría otro investigador?

## Próxima decisión
- Repetir / avanzar (según evidencia):
```

## V. Cómo estudiar en pareja sin confundirse

- Mismo syllabus; **dos Issues individuales** por unidad; no mezclar sus niveles.
- Pueden ver juntos una clase, pero cada uno debe producir su propia explicación y ejecutar comandos.
- Una revisión cruzada semanal; la revisión no equivale a hacer la tarea del otro.
- `PROGRESS.md` resume el estado **solo después** de revisar evidencias: no inventar «completado».
- Preguntas nuevas que no pertenezcan a la unidad: registrar en el Issue como **backlog**, no abandonar la actividad.
- Si una unidad está muy fácil, demostrar la competencia y adelantar; si no, descomponerla.

## VI. Evaluaciones y continuidad

Cada semana: mini defensa de 10–15 minutos por estudiante y revisión del PR.  
Cada cuatro semanas: retrospectiva (prerrequisitos, temas fuertes, errores recurrentes, carga y rumbo).  
Cada ciclo de 12 semanas: un proyecto integrador y defensa técnica.  
Para investigación: incorporar ejercicios matemáticos y lectura de papers gradualmente.

**No estudiar para marcar casillas:** el estándar es ser capaz de explicar, ejecutar, diagnosticar y documentar sin ayudas críticas.
