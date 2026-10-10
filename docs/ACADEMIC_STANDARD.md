# Estándar académico y técnico

## 1. Principio rector

**Una afirmación técnica debe sostenerse con evidencia verificable; una herramienta no equivale a una explicación.**

Antes de aceptar un hallazgo: identificar supuestos, construir un modelo, reproducir evidencia y medir sus limitaciones.

## 2. Jerarquía práctica de fuentes

1. **Primarias:** RFCs de [IETF](https://www.rfc-editor.org/), especificaciones [W3C](https://www.w3.org/TR/), estándares oficiales, documentación de proyectos, código fuente original y publicaciones científicas originales.
2. **Académicas:** publicaciones revisadas por pares, textos técnicos y materiales de cursos de universidades (MIT, CMU y equivalentes). Pueden estar desactualizados: verificar vigencia.
3. **Guías de organizaciones técnicas:** [OWASP](https://owasp.org/), [NIST](https://www.nist.gov/cyberframework), [Ethereum](https://ethereum.org/en/developers/docs/) y documentación de herramientas.
4. **Complementarias:** writeups, foros, blogs, videos y respuestas de IA. Se usan para orientación, pero se contrastan con fuentes superiores.

La fuente idónea depende de la afirmación: un RFC sirve para un protocolo; el código fuente y una prueba sirven para demostrar un fallo de implementación.

## 3. Cómo citar en los apuntes

Usar enlaces Markdown y fecha de consulta cuando la información evoluciona:

```markdown
## Fuentes
1. Autor o institución. "Título". Versión o año.
   URL: https://...
   Secciones consultadas: ...
   Consultado: AAAA-MM-DD.
   Evidencia utilizada: ...
```

Para artículos científicos, agregar DOI o enlace a la versión original cuando exista. **Nunca inventar páginas, DOI, citas textuales ni referencias.**

## 4. Plantilla mínima de laboratorio

- **Pregunta / objetivo:**
- **Prerrequisitos y entorno:** SO, versiones, dependencias.
- **Modelo mental / hipótesis:**
- **Fuente primaria consultada:**
- **Comandos y pasos reproducibles:**
- **Resultado observado:** salida o pruebas, no afirmaciones sin evidencia.
- **Explicación causal:** por qué sucedió.
- **Limitaciones y alternativas:**
- **Corrección / mitigación** (cuando aplique):
- **Preguntas abiertas:**
- **Autor y revisor:**

No guardar contraseñas ni tokens de laboratorios o recursos reales.

## 5. Rúbrica (0–4 por criterio)

| Criterio | 0 | 2 | 4 |
| --- | --- | --- | --- |
| Fundamentos | No explica | Explica parcialmente | Explica mecanismo y supuestos |
| Ejecución | Sin evidencia | Parcialmente reproducible | Completamente reproducible |
| Pensamiento crítico | Copia conclusiones | Identifica algunos límites | Contrasta hipótesis y alternativas |
| Fuentes | Sin fuente | Fuente pertinente incompleta | Fuente primaria bien localizada y citada |
| Comunicación | Incomprensible | Comprensible con lagunas | Informe claro, preciso y revisable |

20 puntos es el máximo, **no es una calificación académica oficial**. Un resultado alto no demuestra maestría de todo un dominio.

## 6. Proyecto de investigación

1. Formular pregunta concreta y falsable.
2. Revisar trabajo previo con referencias.
3. Definir modelo de amenaza o propiedad a verificar.
4. Diseñar herramienta, modelo o experimento.
5. Especificar datasets, entorno, versiones y métricas.
6. Ejecutar, reproducir, comparar y analizar errores.
7. Publicar metodología, limitaciones y referencias.

## 7. Bibliografía inicial con usos específicos

- [CMU — Introduction to Computer Security (2025)](https://www.andrew.cmu.edu/course/18-330/2025s/) — amenazas, software, redes y criptografía.
- [MIT 6.858 — Computer Systems Security (2014)](https://ocw.mit.edu/courses/6-858-computer-systems-security-fall-2014/) — seguridad de sistemas e investigación. **Material histórico; no asumir vigencia de comandos.**
- [CMU — Program Analysis (2025)](https://cmu-program-analysis.github.io/2025/syllabus.html) — análisis estático, symbolic execution y abstract interpretation.
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/) — metodología de evaluación web.
- [Solidity Security Considerations](https://docs.soliditylang.org/en/latest/security-considerations.html) — aspectos de seguridad y diseño de contratos.
- [Ethereum Developers Documentation](https://ethereum.org/en/developers/docs/) — cuentas, transacciones y EVM.

