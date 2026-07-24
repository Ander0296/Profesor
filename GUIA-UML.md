GUÍA: UML DISTILLED (Fowler, 3ra ed.) + POO EN JAVA
No asume conocimiento previo — la mantiene Claude Code sesión a sesión.
Cada sesión cubre una tanda de 3-5 páginas del libro, explicadas en
español y conectadas con código Java. Ejercicios: ver EJERCICIOS.md.
============================================================

INICIO RÁPIDO
------------------------------------------------------------
- Última página estudiada: Ubicación 730 de 3171 (23%) — legal UML, supresión, significado de UML, "UML no alcanza" (Figura 1.3)
- Última sesión: #09
- Ejercicios pendientes: EJERCICIO #01 (screen flow diagram). Estados completos, fechas y repasos: ver EJERCICIOS.md (fuente de verdad; esta línea solo lista lo pendiente).

VOCABULARIO EN <-> ES (Claude agrega una fila por término nuevo)
------------------------------------------------------------
| Inglés                        | Español                          | En una frase                                                        |
|-------------------------------|-----------------------------------|----------------------------------------------------------------------|
| law of parsimony              | ley de la parsimonia              | Reducir todo a su esencia: la forma debe acompañar a la función.    |
| sketch                        | boceto                            | Uso informal de UML para explorar ideas rápido, sin rigor.          |
| blueprint                     | plano                             | Uso preciso de UML: alguien podría construir el sistema solo con él.|
| CRC cards                     | tarjetas CRC                      | Técnica de diseño OO en papel, no es notación UML pura (se ve después).|
| Object Management Group (OMG) | Object Management Group (OMG)     | Consorcio de empresas que controla el estándar UML.                 |
| meta-model                    | meta-modelo                       | El "modelo del modelo": reglas que respaldan toda la notación UML.  |
| UML as sketch                 | UML como boceto                   | Uso selectivo/informal de UML: solo lo importante para discutir.    |
| UML as blueprint               | UML como plano                    | Uso completo/detallado de UML: el programador solo "codifica".      |
| forward engineering            | ingeniería hacia adelante         | Dibujar el diagrama ANTES de escribir el código.                    |
| reverse engineering            | ingeniería inversa                | Armar el diagrama A PARTIR de código que ya existe.                 |
| UML as programming language    | UML como lenguaje de programación | El diagrama SE COMPILA directo a código: diagrama y código son lo mismo.|
| round-trip tools               | herramientas round-trip           | Hacen forward Y reverse engineering, yendo y viniendo.              |
| tripless tools                 | herramientas tripless             | El código ES el repositorio; el diagrama es solo una vista.         |
| Model Driven Architecture (MDA)| MDA                               | Estándar del OMG para usar UML como lenguaje de programación.       |
| Platform Independent Model (PIM)| PIM                              | Modelo UML sin depender de ninguna tecnología concreta.             |
| Platform Specific Model (PSM)  | PSM                               | Modelo dirigido a un entorno de ejecución específico (ej. J2EE).    |
| Executable UML                 | Executable UML                    | Variante de MDA: un model compiler pasa el modelo a sistema en un paso.|
| archetype                      | arquetipo                         | Regla que le dice al model compiler cómo llevar el modelo a una plataforma concreta.|
| software perspective           | perspectiva de software           | Los elementos del diagrama mapean casi directo a elementos de un sistema real.|
| conceptual perspective         | perspectiva conceptual            | El diagrama describe conceptos de un dominio, sin pensar en software.|
| notation                       | notación                          | La sintaxis gráfica de UML: cómo se dibuja cada símbolo.            |
| Three Amigos                   | Los Tres Amigos                   | Booch, Rumbaugh y Jacobson; los más asociados a la creación de UML. |
| Structure Diagram              | Diagrama de Estructura            | Familia de diagramas UML que muestra QUÉ existe (clases, paquetes, etc.).|
| Behavior Diagram               | Diagrama de Comportamiento        | Familia de diagramas UML que muestra QUÉ HACE el sistema.           |
| prescriptive rules             | reglas prescriptivas              | Un organismo oficial dicta qué es legal (ej. lenguajes de programación).|
| descriptive rules              | reglas descriptivas               | Las reglas se entienden por cómo la gente usa el lenguaje en la práctica.|
| suppression                    | supresión                         | Un diagrama puede ocultar info a propósito; ausencia no implica nada.|
| normative / non-normative       | normativo / no normativo          | Normative = obligatorio según el estándar; non-normative = no es estrictamente legal en UML.|

============================================================
(SESIONES — desde la #10 en formato CORTO: 5-8 bullets, sin bloques
de código ni diagramas repetidos, máximo ~15 líneas por sesión. Las
sesiones #01 a #09, en formato largo, están en GUIA-ARCHIVO.md.)
============================================================

============================================================
FORMATO DE CADA SESIÓN (referencia para Claude — copiar y llenar)
Formato CORTO obligatorio: 5-8 bullets, SIN bloques de código ni
diagramas (ya viven en el chat, el libro y los ejercicios), sin
narrar las dudas (solo tema + veredicto en una línea). Máx ~15 líneas.
============================================================

SESIÓN #NN — [fecha] — [tema] (Ubicación X-Y, Z%)
- [idea clave 1, una línea]
- [idea clave 2...]
- Ejercicios de la tanda: [nombre + pendiente/completado, o "ninguno"]
- Nota del profe: [solo si la hubo, una línea]
- Dudas: [tema + bien/corregido en una línea, o "ninguna"]
- PRÓXIMO PASO: [una línea]
