# Roadmap por competencias — Ciberseguridad — Jorge

> Fecha de arranque: octubre de 2026. Los plazos son flexibles. Se avanza al demostrar competencias; no por cumplir un número de días.

## Etapa 0 — Aprender a investigar y usar GitHub

**Tema:** Git, branches, commits, PRs, Markdown, búsqueda de fuentes y citación.

**Evidencia:** primer PR individual, revisado por el mentor o un colaborador, con una nota original y al menos una referencia primaria.

## Etapa 1 — Linux y fundamentos de sistemas

**Temas:** filesystem, shell, permisos, procesos, pipes, redirecciones, SSH, usuarios, logs, servicios y variables de entorno.

**Laboratorios:** [OverTheWire Bandit](https://overthewire.org/wargames/bandit/); [TryHackMe Pre Security](https://tryhackme.com/path/outline/presecurity).

**Evidencia:** resolver y explicar ejercicios; diagnóstico de un error; comando + salida + causa + fuente.

## Etapa 2 — Networking, web y modelos de amenaza

**Temas:** TCP/IP, DNS, TLS, HTTP, cookies, sesiones, CORS, autenticación, autorización, threat modeling.

**Evidencia:** explicar flujo completo de una petición, interceptar tráfico local y modelar amenazas de una API propia.

## Etapa 3 — Web AppSec

**Temas:** OWASP Top 10, SQLi, IDOR, XSS, CSRF, SSRF, race conditions, revisión manual de código, pruebas de regresión.

**Laboratorios:** [PortSwigger Web Security Academy](https://portswigger.net/web-security), [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/).

**Evidencia:** informe técnico verificable con causa raíz, PoC local y mitigación.

## Etapa 4 — EVM, contratos y wallets

**Temas:** Ethereum, transacciones, gas, ABI, storage, Solidity, firmas, EIP-712, Foundry, tests.

**Laboratorios:** [Remix](https://remix.ethereum.org/), [Foundry](https://getfoundry.sh/), [Ethernaut](https://ethernaut.openzeppelin.com/).

**Evidencia:** desarrollar contratos propios, implementar controles y justificar invariantes.

## Etapa 5 — Seguridad económica y auditorías

**Temas:** Reentrancy, access control, oracles, DeFi accounting, vaults, lending, fuzzing, static analysis, invariant testing.

**Laboratorios:** [Damn Vulnerable DeFi](https://github.com/theredguild/damn-vulnerable-defi), Slither, Echidna.

**Evidencia:** evaluación reproducible, código probado y un informe con riesgos residuales.

## Etapa 6 — Ciencia e investigación de seguridad (abierta)

Posibles líneas de especialización:

- **Program analysis:** compiladores, CFG, dataflow, abstract interpretation, static analyzers.
- **Formal methods:** lógica de Hoare, model checking, SMT/SAT, symbolic execution y proof assistants.
- **Criptografía:** matemática discreta, teoría de números, curvas elípticas, protocolos y zero-knowledge.
- **Protocol / DeFi research:** modelos económicos, teoría de juegos, análisis de incentivos y diseño de seguridad.
- **Systems security:** arquitecturas, aislamiento, memory safety, side channels y observabilidad.
- **AI security:** evaluación de modelos, agentes, amenazas a herramientas y seguridad de sistemas con IA.

**Evidencia:** problema original, literatura, hipótesis, implementación, mediciones, límites y reproducción independiente.

## Primer ciclo de trabajo

Seguir el orden de sesiones de [STUDY_PLAN.md](STUDY_PLAN.md). Empezar por terminal y shell; continuar con SSH/Bandit 0, navegación y documentación según evidencia. No fijar niveles Bandit por día ni introducir redes avanzadas antes de los prerrequisitos.

## Registro individual

**Jorge:** pendiente de diagnóstico inicial.  

Cada semana: competencias practicadas, evidencia GitHub, dudas, fuente consultada y siguiente experimento.
