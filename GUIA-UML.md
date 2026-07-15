GUÍA: UML DISTILLED (Fowler, 3ra ed.) + POO EN JAVA
No asume conocimiento previo — la mantiene Claude Code sesión a sesión.
Cada sesión cubre una tanda de 3-5 páginas del libro, explicadas en
español y conectadas con código Java. Ejercicios: ver EJERCICIOS.md.
============================================================

INICIO RÁPIDO
------------------------------------------------------------
- Última página estudiada: Ubicación 553 de 3171 (15%) — fin de "Ways of Using the UML" + MDA + Executable UML
- Última sesión: #05
- Ejercicios pendientes: ver EJERCICIOS.md (ninguno todavía — contenido introductorio, sin conceptos de diagramas aún)

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

============================================================
SESIÓN #01 — 2026-07-11 — Prólogo 3ra edición (Cris Kobryn) (Ubicación 332-358, 6-7%)
============================================================

IDEAS CLAVE
- Ley de la parsimonia: los mejores diseños de la historia (pirámides,
  UNIX, Smalltalk) siguen "menos es más" / Occam's Razor.
- Kobryn presidió la estandarización de UML 2.0 y admite que el proceso
  de comité agregó complejidad gratuita ("design by committee").
  Por eso valora que Fowler haya distilado el 20% de UML que resuelve
  el 80% del trabajo real (principio de Pareto).
- UML tiene dos usos bien distintos: "pararrayos de creatividad"
  (boceto informal) vs. "láser de precisión" (plano tan exacto que un
  tercero podría construir el sistema con eso solo). Esta segunda es
  la "prueba ácida" de un lenguaje de planos genuino.

UML <-> JAVA (cómo se ve cada concepto en código)
- Todavía no aplica — contenido puramente introductorio, sin notación
  UML mostrada aún.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- El 80/20 (Pareto) no es solo filosofía de diagramas: es la regla de
  oro de TODO el código. Sobre-diseñar (agregar interfaces y patrones
  que nadie pidió) es un error típico de junior. Saber cuándo parar es
  señal de senior.

DUDAS QUE SURGIERON (y su respuesta corta)
- Diferencia entre "pararrayos de creatividad" (comunicación informal)
  y "láser de precisión" (plano suficientemente completo para construir
  sin ambigüedad, no solo para que dos personas se entiendan).

EJERCICIOS CREADOS: ninguno (tema introductorio)
PRÓXIMO PASO: Foreword a la 1ra edición + Preface

============================================================
SESIÓN #02 — 2026-07-11 — Foreword 1ra edición + Preface + inicio "Why Bother with the UML?" (Ubicación 362-406, 8-9%)
============================================================

IDEAS CLAVE
- "The Three Amigos" (Booch, Jacobson, Rumbaugh) crearon UML unificando
  tres métodos de modelado OO que competían en los 90. Crear UML fue
  en sí un proceso iterativo e incremental.
- Fowler explica el propósito del libro: deliberadamente breve, busca
  la fracción de UML más útil (mismo concepto 80/20 de la Sesión #01).
  Es un libro CON OPINIÓN (no pretende ser neutral).
- El libro NO enseña OO desde cero (para eso recomienda a Larman) —
  ese hueco lo cubrimos nosotros en el chat.
- Los ejemplos de código del libro son en Java y C#.
- Valor principal de un diagrama: comunicación y entendimiento en
  equipo, no reemplazar el código. Fowler es escéptico de que lo
  gráfico algún día reemplace al texto/código.
- UML se volvió importante por su adopción masiva y estandarización
  dentro (y fuera) del mundo OO.

UML <-> JAVA (cómo se ve cada concepto en código)
- Todavía no aplica — sigue siendo introducción. Dato a retener: los
  próximos ejemplos de código del libro (y los nuestros) van a ser en
  Java.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- Frase para grabar: "UML es un asistente, no un reemplazo del código."
  Se usa para pensar y comunicar antes o en paralelo al código, nunca
  en vez de escribirlo.

DUDAS QUE SURGIERON (y su respuesta corta)
- Ninguna — ambas respuestas de verificación fueron correctas.

EJERCICIOS CREADOS: ninguno (tema introductorio)
PRÓXIMO PASO: seguir "Why Bother with the UML?" y entrar a los primeros
conceptos concretos de UML.

============================================================
SESIÓN #03 — 2026-07-11 — Acknowledgments (Ubicación 449-485, 11-12%)
============================================================

IDEAS CLAVE
- Sección de agradecimientos de Fowler, sin contenido técnico nuevo.
- Craig Larman reaparece como revisor (mismo autor recomendado antes
  para aprender OO desde cero).

UML <-> JAVA (cómo se ve cada concepto en código)
- No aplica.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- Ninguna esta vez.

DUDAS QUE SURGIERON (y su respuesta corta)
- Ninguna — tanda sin contenido conceptual, no se hizo verificación.

EJERCICIOS CREADOS: ninguno
PRÓXIMO PASO: arranca el cuerpo del libro — primeros conceptos
concretos de UML.

============================================================
SESIÓN #04 — 2026-07-11 — Cap. 1 Introducción: "What Is the UML?" + arranca "Ways of Using the UML" (Ubicación 487-513, 12-14%)
============================================================

IDEAS CLAVE
- UML = familia de notaciones gráficas respaldadas por un único
  meta-modelo, para describir/diseñar sistemas OO. Existe porque el
  código no tiene nivel de abstracción suficiente para discutir diseño.
- UML lo controla el OMG (Object Management Group), conocido también
  por CORBA. Nació unificando varios lenguajes gráficos OO de fines
  de los 80/principios de los 90.
- Fowler y Steve Mellor identificaron 3 formas de usar UML: sketch,
  blueprint y programming language (el 3ro todavía no se vio).
- Sketch (boceto) = selectivo/informal, mostrás solo lo importante.
  Blueprint (plano) = completo/detallado, el programador solo codifica
  lo que el diseñador ya decidió.
- Forward engineering (diagrama antes del código) y reverse engineering
  (diagrama a partir del código ya existente) son un EJE INDEPENDIENTE:
  tanto sketch como blueprint pueden hacerse en cualquiera de las dos
  direcciones.
- La mayoría de los diagramas de este libro (y de la mayoría de los
  libros) son bocetos, no planos completos.

UML <-> JAVA (cómo se ve cada concepto en código)
- Todavía sin notación concreta de diagramas. Se conectó con el propio
  flujo de trabajo del proyecto: diseñar en el chat antes de escribir
  código en ejercicios/ = forward engineering + sketch; diagramar en
  diagramas/*.puml a partir de código ya escrito = reverse engineering
  + sketch.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- Sketch vs. blueprint es probablemente el concepto más citado del
  libro y sale en entrevistas técnicas. En la industria real casi
  nadie hace "blueprint" completo — se usa mucho más como boceto
  rápido de pizarra para alinear al equipo antes de codear.

DUDAS QUE SURGIERON (y su respuesta corta)
- Confusión inicial: pensar que "sketch" se define por ser hecho A
  PARTIR del código (reverse). Corrección: sketch/blueprint (qué tan
  completo) y forward/reverse (en qué dirección) son dos ejes
  independientes — ambos modos admiten las dos direcciones.

EJERCICIOS CREADOS: ninguno todavía
PRÓXIMO PASO: tercer modo "UML as programming language" y seguir
Capítulo 1.

============================================================
SESIÓN #05 — 2026-07-11 — Cierre "Ways of Using the UML" + MDA + Executable UML (Ubicación 525-553, 14-15%)
============================================================

IDEAS CLAVE
- Blueprint puede ser parcial (solo interfaces de subsistemas) o total.
  En reverse engineering, un blueprint muestra el detalle de una clase
  en forma gráfica.
- Herramientas CASE (término hoy evitado por sobreventa de los 90):
  forward-engineering tools, reverse-engineering tools, round-trip
  tools (hacen ambas), y "tripless tools" (el código ES el repositorio,
  el diagrama es solo una vista).
- Frase resumen: "los bocetos son exploratorios, los planos son
  definitivos."
- 3er modo: UML as programming language — el diagrama se compila
  directo a código ejecutable; diagrama y código son la misma cosa,
  por eso forward/reverse engineering dejan de tener sentido ahí.
- MDA (Model Driven Architecture, estándar del OMG): PIM (modelo
  independiente de plataforma) -> PSM (modelo específico de una
  plataforma) -> código. Si todo el proceso es automático = UML as
  programming language; si algún paso es manual = blueprint.
- Executable UML (Mellor): salta el PSM, usa un "model compiler" +
  "archetypes" para ir directo de modelo a sistema desplegable en un
  paso automático. Usa menos construcciones que el UML completo.

UML <-> JAVA (cómo se ve cada concepto en código)
- Conexión directa con este proyecto: siempre vamos a trabajar en modo
  "UML as sketch" — nunca se compila un diagrama a Java acá, el
  usuario escribe todo el código a mano.

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- MDA y Executable UML son nicho (embebidos, aeroespacial,
  telecomunicaciones) y no hace falta memorizarlos para el primer
  laburo. Lo que sí hay que tener sólido es la distinción
  sketch / blueprint / programming language.

DUDAS QUE SURGIERON (y su respuesta corta)
- Ninguna — ambas respuestas de verificación fueron correctas al
  primer intento.

EJERCICIOS CREADOS: ninguno todavía
PRÓXIMO PASO: seguir Capítulo 1 — próximos temas de la introducción.

============================================================
FORMATO DE CADA SESIÓN (referencia para Claude — copiar y llenar)
============================================================
SESIÓN #NN — [fecha] — [tema] (páginas X-Y del libro)

IDEAS CLAVE
- ...

UML <-> JAVA (cómo se ve cada concepto en código)
- ...

NOTA DEL PROFE (cosas que el libro no dice pero importan)
- ...

DUDAS QUE SURGIERON (y su respuesta corta)
- ...

EJERCICIOS CREADOS: #...
PRÓXIMO PASO: ...
