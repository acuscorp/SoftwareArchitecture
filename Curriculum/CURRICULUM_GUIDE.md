# Guía para generar clases — Arquitectura de Software

> Esta guía conserva únicamente el marco de generación de clases: propósito, jerarquía, resultados y prerrequisitos curriculares, alcance por módulo/clase, consulta de fuentes, evidencia, limitaciones y condiciones de revisión. La [ruta tabular](LEARNING_PATH.md) es la referencia canónica para el título de cada clase y sus fuentes/capítulos. Ninguna regla aquí convierte por sí sola un plan en aprobado.

## Índice

1. [Propósito y perfil de entrada](#1-proposito-y-perfil-de-entrada)
2. [Instrucciones de diseño y organización](#2-jerarquia-curricular-y-reglas-de-organizacion)
3. [Mapa de módulos, prerrequisitos y resultados](#3-mapa-de-modulos-prerrequisitos-y-evidencias)
4. [Índice de clases, alcances y fronteras](#4-indice-detallado-de-clases)
5. [Prerrequisitos y progresión](#5-prerrequisitos-y-reglas-de-avance)
6. [Evidencia y evaluación](#6-evaluacion-y-evidencia-de-dominio)
7. [Limitaciones y condiciones de revisión](#7-limitaciones-y-condiciones-de-revision)

## 1. Propósito y perfil de entrada

### Identidad del curso

- `course_id`: `SAC01`
- Este identificador establece la identidad del curso; no implica por sí solo aprobación curricular ni migración del progreso.
- La [matriz maestra de competencias](MATRIZ_COMPETENCIAS.md) es la fuente de referencia para Software Architecture y AI Solution Architecture. Conserva el estado `DRAFT — PENDING_REVIEW`; este vínculo no la aprueba.

### Propósito y alcance

La ruta tabular `LEARNING_PATH.md` es el índice de consulta por clase. Esta guía conserva la jerarquía y los criterios curriculares detallados. La jerarquía oficial es **Módulo → Submódulo → Clase → Subclase (cuando aplique)**. Los 15 módulos mantienen la correspondencia uno a uno con los 15 bloques de la ruta base. Los submódulos organizan áreas temáticas; cada clase queda delimitada por su título y por una cantidad acotada de subclases (unidades de aprendizaje). El resultado de aprendizaje específico, la actividad y el criterio de evaluación se concretarán en el plan de esa clase.

La estructura curricular organiza las unidades de aprendizaje dentro de las clases y separa algunas unidades que combinaban resultados distintos. La división detallada es una organización curricular derivada de la ruta base, no una transcripción literal de ella. La ruta no declara dominio del estudiante, no contiene explicaciones de clase ni sustituye los planes didácticos.

**Perfil de entrada:** esta ruta no especifica un perfil de entrada global de forma independiente. No se infiere uno; deberá concretarse mediante diagnóstico o acuerdo de tutoría antes de personalizar la progresión.

## 2. Instrucciones de diseño y organización

### Convenciones de jerarquía e identificadores

- **Módulo `M01`–`M15`:** corresponde al bloque numerado de la ruta anterior.
- **Submódulo `SM01.01`:** mantiene la numeración temática (por ejemplo, `SM04.05` corresponde al tema 4.5).
- **Clase `CL04.05.01`:** identificador estable de la primera clase del submódulo 4.5. Las clases se numeran dentro de cada submódulo.
- **Subclase `SCL04.05.01.01`:** unidad específica de contenido dentro de una clase. Se crea para hacer explícito el alcance, no necesariamente para impartirse como una sesión independiente.
- Los antiguos `Subtema x.y.z` pasan a ser subclases numeradas. Los antiguos títulos `Clase x.y` se conservan como referencia histórica en el registro de migración.
- El índice usa el término **clase** para una unidad de enseñanza planificable. Meta de diseño: **60–90 minutos por clase**, ajustable según el plan didáctico. Si una clase necesita más de tres subclases conceptualmente distintas, se divide o se diseña explícitamente como secuencia; no se sobrecarga por mantener una sola sesión.
- Las subclases identifican qué debe cubrirse; las actividades, criterios de evaluación y evidencias se definen en documentos de clase separados. Al diseñar cada clase, es obligatorio consultar las fuentes asignadas en la ruta tabular, revisar el contenido pertinente y cotejar título, edición, capítulo/subcapítulo y páginas con la copia disponible. Si no se puede verificar una referencia o no cubre el objetivo, se registra la limitación y no se inventan páginas ni cobertura. Las fuentes son obligatorias para fundamentar el diseño, no lectura obligatoria para el estudiante salvo que el plan lo indique explícitamente.
- Las referencias cruzadas indican aplicación o profundización, no repetición completa. El mismo concepto puede reaparecer con un propósito distinto, que debe quedar expresado en la frontera del submódulo.

### Fronteras críticas entre módulos

- **M01 vs. M02:** M01 reconoce una decisión de impacto arquitectónico; M02 desarrolla el método de drivers, escenarios, riesgos, alternativas y trade-offs.
- **SM01.02 vs. SM03.05:** M01 da un vocabulario introductorio de estructura/runtime/vistas; M03 enseña a seleccionar y mantener vistas y modelos coherentes.
- **M02 vs. M14:** M02 justifica una decisión concreta con criterios iniciales; M14 evalúa candidatas de manera sistemática, basada en evidencia y con análisis económico/sensibilidad.
- **M06 vs. M07 vs. M10:** M06 define límites semánticos y motivación de dominio; M07 trata interacción y coordinación entre nodos; M10 trata propiedad, persistencia y consistencia dentro de límites de datos.
- **M07 vs. M11:** M07 explica la semántica y mecanismos de fallos distribuidos; M11 define objetivos, controles y prácticas operativas transversales de disponibilidad y recuperación.
- **M09 vs. M11:** M09 protege, prueba y observa el contrato desde el límite API; M11 trata identidad, amenazas y observabilidad/operación del sistema en conjunto.
- **M06 vs. SM10.04:** M06 presenta CQRS/event sourcing solo como posibilidades derivadas del dominio; M10 estudia consecuencias técnicas y trade-offs como patrones de datos.
- **M15:** integra y comunica conocimiento previo; no reenseña técnicas ni reemplaza la evaluación técnica/económica de M14.

---

## 3. Mapa de módulos, prerrequisitos y resultados

### Criterios de progresión y dominio

La progresión de competencias sigue **identificar → explicar → justificar → aplicar**. Los prerrequisitos que aparecen abajo son condiciones mínimas observables de entrada, no requisitos de dominio profundo. Para aprobar cada clase, el plan didáctico deberá especificar una evidencia observable alineada con la competencia; el índice no declara evidencia ya conseguida.

| Módulo | Función principal | Prerrequisito mínimo / entrada observable | Resultado esperado de salida |
|---|---|---|---|
| M01. Pensamiento arquitectónico y fundamentos | Vocabulario, estructura, contexto y reconocimiento de decisiones. | Ninguno. Reconoce al menos un componente, una relación y una preocupación del sistema en un caso sencillo. | **C01–C02:** Explicar arquitectura, estructuras, comportamiento y distinguir una decisión arquitectónica de una decisión local. |
| M02. Requisitos, atributos de calidad, riesgos y decisiones | Drivers, escenarios, riesgos y decisión arquitectónica inicial. | M01: vocabulario de arquitectura y decisiones. Explica una necesidad y distingue funcionalidad, calidad, restricción y riesgo. | **C03–C05:** Formular drivers y escenarios; identificar riesgos; justificar una decisión inicial comparando alternativas. |
| M03. Modelado, diseño orientado a objetos y comunicación arquitectónica | Modelos, notación, vistas y comunicación técnica. | M01–M02: reconocer estructura, decisiones y preocupaciones de calidad. Selecciona qué representar y para qué audiencia; no requiere dominar UML por completo. | **C06:** Crear modelos y vistas que respondan a una preocupación concreta, con notación adecuada. |
| M04. Diseño de módulos, cohesión, acoplamiento y evolución del código | Diseño modular, cohesión, acoplamiento y evolución de código. | M01–M03: leer estructura y modelos básicos. Identifica módulos, responsabilidades y una dependencia en código o un diagrama. | **C07:** Diagnosticar diseño interno y proponer una refactorización o un límite modular justificable. |
| M05. Patrones de diseño y mecanismos de variabilidad | Patrones de diseño de objetos y variabilidad. | M03–M04: objetos, interfaces, composición, cohesión y acoplamiento básicos. Explica un diseño interno y el cambio que intenta facilitar. | **C08:** Seleccionar o descartar un patrón por contexto, fuerzas y consecuencias. |
| M06. Dominio, límites y diseño orientado al negocio | Modelo de dominio, bounded contexts e integración semántica. | M01–M04: estructuras, modularidad y diseño OO básicos. Distingue reglas de negocio de mecanismos técnicos y puede describir términos del dominio. | **C09:** Delimitar modelos y contextos de dominio, justificando sus relaciones y propiedad de conceptos/datos. |
| M07. Arquitecturas y sistemas distribuidos | Comunicación, consistencia, coordinación y fallos distribuidos. | M02 y M04: drivers, trade-offs y contratos/módulos; M06 solo hasta límites de dominio básicos. Identifica dos componentes que se comunican y una consecuencia de latencia o fallo parcial. | **C10:** Comparar comunicación, consistencia, coordinación y mecanismos de tolerancia a fallos. |
| M08. Estilos arquitectónicos y descomposición | Estilos arquitectónicos y estrategia de descomposición. | M02, M04 y M06; M07 solo para reconocer costes básicos de distribución. Compara al menos dos formas de desplegar/descomponer sin asumir que microservicios son la opción por defecto. | **C11:** Justificar la forma de descomposición y las unidades de despliegue frente a restricciones del caso. |
| M09. APIs como arquitectura | Contratos API, compatibilidad, gestión y evolución. | M02–M03; nociones básicas de límites y dependencias de M06–M08. Describe consumidor, productor, operación/dato intercambiado y expectativa de compatibilidad. | **C12:** Definir contratos API utilizables, compatibles, protegibles y observables. |
| M10. Datos, persistencia y consistencia arquitectónica | Propiedad, persistencia, integridad y patrones de datos. | M02, M04 y M06; nociones de comunicación/consistencia de M07. Identifica quién es dueño de un dato, quién lo consume y una invariante que debe protegerse. | **C13:** Justificar propiedad, persistencia y patrones de datos mediante consistencia, operación y trade-offs. |
| M11. Seguridad, resiliencia, observabilidad y operación | Seguridad, resiliencia, observabilidad y operación transversal. | M02 y nociones aplicables de M07, M09 y M10. Nombra un activo/servicio, una amenaza o modo de fallo y una señal observable. | **C14:** Identificar amenazas y fallos transversales y proponer controles, observabilidad y recuperación. |
| M12. Cloud, despliegue y arquitectura evolutiva | Cloud, despliegue, migración y verificación evolutiva. | M02, M08 y M11: drivers, descomposición y controles/operación básicos. Describe una propiedad que debe conservarse al desplegar o migrar y un criterio de éxito. | **C15:** Proponer una estrategia cloud/despliegue/evolución con reversibilidad y criterios de verificación. |
| M13. Arquitectura para AI Engineering | Arquitectura, evaluación y operación de aplicaciones AI. | M02 como obligatorio; M07, M09, M10, M11 y M12 se exigen según los límites elegidos en el caso, no todos en profundidad. Explica el caso de uso, los datos, el límite de integración y cómo se juzgará la calidad del resultado AI. | **C16:** Diseñar una aplicación que integre modelos, datos y sistemas existentes, definiendo evaluación y operación. |
| M14. Evaluación arquitectónica y análisis económico | Comparación sistemática, evidencia y análisis económico. | Drivers y alternativas de M02; se reutiliza el contenido técnico pertinente de M03–M13 según el caso evaluado. Explica una decisión candidata, sus criterios y al menos una incertidumbre relevante. | **C17:** Comparar arquitecturas con evidencia, sensibilidad, costes y riesgos. |
| M15. Práctica profesional del arquitecto | Comunicación profesional, gobernanza y defensa de decisiones. | M01–M14: conocimiento aplicable al caso; no se requiere dominio profundo de todos los temas posibles. Presenta un caso, sus stakeholders, restricciones y decisión pendiente; reconoce evidencia incompleta. | **C18:** Comunicar y defender una propuesta integral ante stakeholders, dejando trazabilidad de decisiones y límites de evidencia. |

## 4. Índice de clases, alcances y fronteras

La jerarquía y los IDs se conservan exactamente en la ruta tabular. Cada clase nueva o revisada debe documentarse con los nueve apartados obligatorios de la [plantilla de plan de clase](../Classes/CLASS_PLAN_TEMPLATE.md). Al diseñarla, se consultan y verifican las fuentes de la ruta tabular y de la ruta tabular conforme a las reglas de consulta de fuentes; sus referencias son orientación para el diseño y no lectura obligatoria del estudiante salvo asignación explícita en el plan. Esta guía no certifica dominio.

### Módulo M01 — Pensamiento arquitectónico y fundamentos

**Alcance:** vocabulario arquitectónico básico, estructura, comportamiento, contexto y reconocimiento inicial de decisiones. **No incluye:** el análisis completo de atributos de calidad, riesgos y trade-offs, que corresponde al bloque 2.

**Competencia principal:** C01–C02. Explicar arquitectura, estructuras, comportamiento y distinguir una decisión arquitectónica de una decisión local.

#### Submódulo SM01.01 — Concepto y propósito de la arquitectura

##### Clase CL01.01.01 — Concepto y propósito de la arquitectura
**Referencia anterior:** Clase 1.1 — Qué es realmente la arquitectura de software.

- **Subclase SCL01.01.01.01:** Qué es la arquitectura de software.
- **Subclase SCL01.01.01.02:** Abstracción y decisiones que condicionan el sistema.
- **Subclase SCL01.01.01.03:** Por qué importa la arquitectura.

#### Submódulo SM01.02 — Estructura y comportamiento de un sistema

##### Clase CL01.02.01 — Distinguir elementos, responsabilidades y relaciones
**Referencia anterior:** Clase 1.2 — Cómo describir la estructura y el comportamiento de un sistema (unidad dividida; véase tabla de migración).

- **Subclase SCL01.02.01.01:** Elementos y responsabilidades.
- **Subclase SCL01.02.01.02:** Relaciones, dependencias y propiedades.

##### Clase CL01.02.02 — Conectar estructura, runtime y vistas introductorias
**Referencia anterior:** Clase 1.2 — Cómo describir la estructura y el comportamiento de un sistema (unidad dividida; véase tabla de migración).

- **Subclase SCL01.02.02.01:** Estructura estática y comportamiento en tiempo de ejecución.
- **Subclase SCL01.02.02.02:** Estructuras y vistas arquitectónicas.

#### Submódulo SM01.03 — Arquitectura, diseño e implementación

##### Clase CL01.03.01 — Arquitectura, diseño e implementación
**Referencia anterior:** Clase 1.3 — Distinguir arquitectura, diseño e implementación.

- **Subclase SCL01.03.01.01:** Diferencias de alcance y nivel de decisión.
- **Subclase SCL01.03.01.02:** Cambios locales frente a cambios con impacto arquitectónico.

#### Submódulo SM01.04 — Contexto y participantes

##### Clase CL01.04.01 — Contexto y participantes
**Referencia anterior:** Clase 1.4 — Reconocer el contexto y las preocupaciones que condicionan la arquitectura.

- **Subclase SCL01.04.01.01:** Identificar stakeholders y sus preocupaciones principales.
- **Subclase SCL01.04.01.02:** Contexto, restricciones y límites iniciales del sistema.

#### Submódulo SM01.05 — Decisiones arquitectónicas

##### Clase CL01.05.01 — Decisiones arquitectónicas
**Referencia anterior:** Clase 1.5 — Reconocer cuándo una decisión tiene impacto arquitectónico.

- **Subclase SCL01.05.01.01:** Reconocer qué decisiones afectan la estructura o propiedades del sistema.
- **Subclase SCL01.05.01.02:** Identificar consecuencias iniciales de una decisión.

---

### Módulo M02 — Requisitos, atributos de calidad, riesgos y decisiones

**Alcance:** el proceso inicial para pasar de necesidades a drivers, escenarios, riesgos y una decisión razonada. **No incluye:** evaluación económica formal ni comparación integral de arquitecturas, que corresponde al bloque 14.

**Competencia principal:** C03–C05. Formular drivers y escenarios; identificar riesgos; justificar una decisión inicial comparando alternativas.

#### Submódulo SM02.01 — Necesidades y requisitos

##### Clase CL02.01.01 — Necesidades y requisitos
**Referencia anterior:** Clase 2.1 — Distinguir requisitos, atributos de calidad y restricciones.

- **Subclase SCL02.01.01.01:** Requisitos funcionales.
- **Subclase SCL02.01.01.02:** Atributos de calidad y requisitos no funcionales.
- **Subclase SCL02.01.01.03:** Restricciones y contexto de negocio/técnico.

#### Submódulo SM02.02 — Drivers arquitectónicos

##### Clase CL02.02.01 — Drivers arquitectónicos
**Referencia anterior:** Clase 2.2 — De requisitos a drivers arquitectónicos.

- **Subclase SCL02.02.01.01:** Requisitos arquitectónicamente significativos (ASR).
- **Subclase SCL02.02.01.02:** Relación entre necesidad, requisito, atributo, restricción y driver.
- **Subclase SCL02.02.01.03:** Priorizar los drivers relevantes para una decisión.

#### Submódulo SM02.03 — Escenarios de calidad

##### Clase CL02.03.01 — Escenarios de calidad
**Referencia anterior:** Clase 2.3 — Formular escenarios de atributos de calidad.

- **Subclase SCL02.03.01.01:** Fuente, estímulo y entorno.
- **Subclase SCL02.03.01.02:** Artefacto, respuesta y medida de respuesta.
- **Subclase SCL02.03.01.03:** Convertir necesidades vagas en criterios evaluables.

#### Submódulo SM02.04 — Riesgo arquitectónico

##### Clase CL02.04.01 — Riesgo arquitectónico
**Referencia anterior:** Clase 2.4 — Razonar sobre riesgos antes de elegir una solución.

- **Subclase SCL02.04.01.01:** Identificación y priorización de riesgos.
- **Subclase SCL02.04.01.02:** Relación entre riesgo, drivers y decisiones.
- **Subclase SCL02.04.01.03:** Selección de técnicas y evaluación de mitigación.

#### Submódulo SM02.05 — Alternativas y trade-offs

*Frontera:* aquí se aprende a construir y justificar una decisión concreta; la evaluación comparativa sistemática y el análisis económico se reservan para el bloque 14.

##### Clase CL02.05.01 — Generar alternativas arquitectónicas viables
**Referencia anterior:** Clase 2.5 — Comparar alternativas y justificar una decisión (unidad dividida; véase tabla de migración).

- **Subclase SCL02.05.01.01:** Generar alternativas viables.

##### Clase CL02.05.02 — Comparar consecuencias y registrar una decisión
**Referencia anterior:** Clase 2.5 — Comparar alternativas y justificar una decisión (unidad dividida; véase tabla de migración).

- **Subclase SCL02.05.02.01:** Beneficios, costes, consecuencias e incertidumbre.
- **Subclase SCL02.05.02.02:** Comparar alternativas con criterios explícitos.
- **Subclase SCL02.05.02.03:** Decisiones arquitectónicas y registros de decisión (ADR).

---

### Módulo M03 — Modelado, diseño orientado a objetos y comunicación arquitectónica

**Alcance:** modelos técnicos y vistas usadas para comprender y representar estructura y comportamiento. **No incluye:** negociación con stakeholders ni gobernanza documental, que corresponden al bloque 15.

**Competencia principal:** C06. Crear modelos y vistas que respondan a una preocupación concreta, con notación adecuada.

#### Submódulo SM03.01 — Fundamentos de modelado

##### Clase CL03.01.01 — Fundamentos de modelado
**Referencia anterior:** Clase 3.1 — Modelar para comunicar una preocupación concreta.

- **Subclase SCL03.01.01.01:** Propósito y alcance de un modelo.
- **Subclase SCL03.01.01.02:** Elegir qué información mostrar según la audiencia.

#### Submódulo SM03.02 — Orientación a objetos

##### Clase CL03.02.01 — Orientación a objetos
**Referencia anterior:** Clase 3.2 — Reconocer elementos y relaciones del diseño orientado a objetos.

- **Subclase SCL03.02.01.01:** Objetos, clases y responsabilidades.
- **Subclase SCL03.02.01.02:** Interfaces, asociaciones, herencia y composición.

#### Submódulo SM03.03 — UML estructural

##### Clase CL03.03.01 — Diagramas de clases
**Referencia anterior:** Clase 3.3 — Representar estructura con UML (unidad dividida; véase tabla de migración).

- **Subclase SCL03.03.01.01:** Diagramas de clases.

##### Clase CL03.03.02 — Diagramas de componentes
**Referencia anterior:** Clase 3.3 — Representar estructura con UML (unidad dividida; véase tabla de migración).

- **Subclase SCL03.03.02.01:** Diagramas de componentes.

##### Clase CL03.03.03 — Diagramas de despliegue
**Referencia anterior:** Clase 3.3 — Representar estructura con UML (unidad dividida; véase tabla de migración).

- **Subclase SCL03.03.03.01:** Diagramas de despliegue.

#### Submódulo SM03.04 — UML de comportamiento

##### Clase CL03.04.01 — UML de comportamiento
**Referencia anterior:** Clase 3.4 — Representar interacciones y comportamiento con UML.

- **Subclase SCL03.04.01.01:** Casos de uso.
- **Subclase SCL03.04.01.02:** Diagramas de secuencia.
- **Subclase SCL03.04.01.03:** Diagramas de estados y actividades.

#### Submódulo SM03.05 — Vistas y documentación arquitectónica

##### Clase CL03.05.01 — Vistas y documentación arquitectónica
**Referencia anterior:** Clase 3.5 — Representar una arquitectura mediante vistas coherentes.

- **Subclase SCL03.05.01.01:** Vistas arquitectónicas asociadas a preocupaciones concretas.
- **Subclase SCL03.05.01.02:** Coherencia entre requisitos, modelos y decisiones.

---

### Módulo M04 — Diseño de módulos, cohesión, acoplamiento y evolución del código

**Alcance:** calidad y evolución del diseño dentro del código y de los límites de módulos. **No incluye:** descomposición en servicios, contratos externos de API ni coordinación distribuida, que se tratan en los bloques 8, 9 y 7.

**Competencia principal:** C07. Diagnosticar diseño interno y proponer una refactorización o un límite modular justificable.

#### Submódulo SM04.01 — Modularidad

##### Clase CL04.01.01 — Modularidad
**Referencia anterior:** Clase 4.1 — Evaluar y diseñar módulos.

- **Subclase SCL04.01.01.01:** Módulos, responsabilidades y límites.
- **Subclase SCL04.01.01.02:** Descomposición y ocultamiento de información.

#### Submódulo SM04.02 — Cohesión y acoplamiento

##### Clase CL04.02.01 — Cohesión y acoplamiento
**Referencia anterior:** Clase 4.2 — Identificar problemas de cohesión y acoplamiento.

- **Subclase SCL04.02.01.01:** Cohesión y agrupación de responsabilidades.
- **Subclase SCL04.02.01.02:** Formas y consecuencias del acoplamiento.
- **Subclase SCL04.02.01.03:** Dependencias estáticas y dinámicas.

#### Submódulo SM04.03 — Calidad del diseño existente

##### Clase CL04.03.01 — Calidad del diseño existente
**Referencia anterior:** Clase 4.3 — Diagnosticar problemas de diseño en código existente.

- **Subclase SCL04.03.01.01:** Señales de deterioro y malos olores de código.
- **Subclase SCL04.03.01.02:** Efectos sobre mantenibilidad y evolución.

#### Submódulo SM04.04 — Refactorización y diseño evolutivo

##### Clase CL04.04.01 — Refactorización y diseño evolutivo
**Referencia anterior:** Clase 4.4 — Mejorar el diseño mediante refactorización.

- **Subclase SCL04.04.01.01:** Refactorizar preservando el comportamiento.
- **Subclase SCL04.04.01.02:** Pruebas como red de seguridad.
- **Subclase SCL04.04.01.03:** Evaluar beneficios, riesgos y efectos secundarios.

#### Submódulo SM04.05 — Construcción de software y diseño de interfaces

##### Clase CL04.05.01 — Encapsulación, composición y diseño de unidades
**Referencia anterior:** Clase 4.5 — Aplicar prácticas de construcción que favorecen la corrección y la evolución (unidad dividida; véase tabla de migración).

- **Subclase SCL04.05.01.01:** Rutinas, clases, encapsulación y composición.

##### Clase CL04.05.02 — Interfaces y contratos entre módulos
**Referencia anterior:** Clase 4.5 — Aplicar prácticas de construcción que favorecen la corrección y la evolución (unidad dividida; véase tabla de migración).

- **Subclase SCL04.05.02.01:** Interfaces y contratos internos entre módulos.

##### Clase CL04.05.03 — Concurrencia, datos compartidos y errores
**Referencia anterior:** Clase 4.5 — Aplicar prácticas de construcción que favorecen la corrección y la evolución (unidad dividida; véase tabla de migración).

- **Subclase SCL04.05.03.01:** Concurrencia, datos compartidos y manejo de errores a nivel de código.

---

### Módulo M05 — Patrones de diseño y mecanismos de variabilidad

**Alcance:** patrones orientados al diseño de objetos, responsabilidades y variabilidad interna. **No incluye:** estilos arquitectónicos de sistema, que corresponden al bloque 8.

**Competencia principal:** C08. Seleccionar o descartar un patrón por contexto, fuerzas y consecuencias.

#### Submódulo SM05.01 — Fundamentos de patrones

##### Clase CL05.01.01 — Fundamentos de patrones
**Referencia anterior:** Clase 5.1 — Cuándo un patrón ayuda y cuándo no.

- **Subclase SCL05.01.01.01:** Problema recurrente, contexto y fuerzas.
- **Subclase SCL05.01.01.02:** Consecuencias y costes de aplicar un patrón.
- **Subclase SCL05.01.01.03:** Selección y uso razonado de patrones.

#### Submódulo SM05.02 — Patrones creacionales

##### Clase CL05.02.01 — Patrones creacionales
**Referencia anterior:** Clase 5.2 — Resolver problemas de creación con patrones.

- **Subclase SCL05.02.01.01:** Encapsular decisiones de creación.
- **Subclase SCL05.02.01.02:** Familias de objetos y construcción configurable.

#### Submódulo SM05.03 — Patrones estructurales

##### Clase CL05.03.01 — Patrones estructurales
**Referencia anterior:** Clase 5.3 — Resolver problemas estructurales con patrones.

- **Subclase SCL05.03.01.01:** Composición de objetos y estructuras.
- **Subclase SCL05.03.01.02:** Adaptación, fachadas y delegación.

#### Submódulo SM05.04 — Patrones de comportamiento

##### Clase CL05.04.01 — Patrones de comportamiento
**Referencia anterior:** Clase 5.4 — Resolver problemas de comportamiento con patrones.

- **Subclase SCL05.04.01.01:** Distribución de responsabilidades y algoritmos.
- **Subclase SCL05.04.01.02:** Comunicación y coordinación entre objetos.

#### Submódulo SM05.05 — Variabilidad y selección de patrones

##### Clase CL05.05.01 — Variabilidad y selección de patrones
**Referencia anterior:** Clase 5.5 — Elegir patrones por sus fuerzas y consecuencias.

- **Subclase SCL05.05.01.01:** Diseñar para cambios concretos.
- **Subclase SCL05.05.01.02:** Comparar patrón, solución simple y refactorización futura.

---

### Módulo M06 — Dominio, límites y diseño orientado al negocio

**Alcance:** comprensión del negocio, modelos de dominio y límites de contextos. **No incluye:** protocolos detallados de coordinación distribuida ni estrategias de almacenamiento, que se profundizan en los bloques 7 y 10.

**Competencia principal:** C09. Delimitar modelos y contextos de dominio, justificando sus relaciones y propiedad de conceptos/datos.

#### Submódulo SM06.01 — Dominio y subdominios

##### Clase CL06.01.01 — Dominio y subdominios
**Referencia anterior:** Clase 6.1 — Identificar el dominio y sus subdominios.

- **Subclase SCL06.01.01.01:** Dominio, subdominio y core domain.
- **Subclase SCL06.01.01.02:** Lenguaje y conocimiento del negocio.

#### Submódulo SM06.02 — Bounded contexts y context maps

##### Clase CL06.02.01 — Bounded contexts y context maps
**Referencia anterior:** Clase 6.2 — Delimitar contextos y representar sus relaciones.

- **Subclase SCL06.02.01.01:** Límites de contexto y modelos consistentes.
- **Subclase SCL06.02.01.02:** Relaciones e integración entre contextos.

#### Submódulo SM06.03 — Modelos de dominio

##### Clase CL06.03.01 — Modelos de dominio
**Referencia anterior:** Clase 6.3 — Construir un modelo de dominio con límites claros.

- **Subclase SCL06.03.01.01:** Entidades y objetos de valor.
- **Subclase SCL06.03.01.02:** Servicios de dominio y de aplicación.
- **Subclase SCL06.03.01.03:** Agregados e invariantes.

#### Submódulo SM06.04 — Integración orientada al dominio

##### Clase CL06.04.01 — Integración orientada al dominio
**Referencia anterior:** Clase 6.4 — Relacionar los límites del dominio con las opciones de integración.

- **Subclase SCL06.04.01.01:** Eventos de dominio y relaciones de integración entre contextos.
- **Subclase SCL06.04.01.02:** Reconocer CQRS y event sourcing como patrones especializados, sin profundizar aquí en su arquitectura de datos.
- **Subclase SCL06.04.01.03:** Consecuencias de los límites del dominio sobre los contratos y la propiedad de datos.

---

### Módulo M07 — Arquitecturas y sistemas distribuidos

**Alcance:** comunicación, coordinación, consistencia y tolerancia a fallos entre componentes distribuidos. **No incluye:** el catálogo transversal de amenazas, identidad y observabilidad operacional, que corresponde al bloque 11.

**Competencia principal:** C10. Comparar comunicación, consistencia, coordinación y mecanismos de tolerancia a fallos.

#### Submódulo SM07.01 — Fundamentos de distribución

##### Clase CL07.01.01 — Fundamentos de distribución
**Referencia anterior:** Clase 7.1 — Entender los costes y riesgos de la distribución.

- **Subclase SCL07.01.01.01:** Qué cambia al distribuir un sistema.
- **Subclase SCL07.01.01.02:** Latencia, fallos parciales y coordinación.

#### Submódulo SM07.02 — Comunicación entre componentes distribuidos

##### Clase CL07.02.01 — Comunicación entre componentes distribuidos
**Referencia anterior:** Clase 7.2 — Comparar mecanismos de comunicación distribuida.

- **Subclase SCL07.02.01.01:** Comunicación síncrona y asíncrona.
- **Subclase SCL07.02.01.02:** Brokers, mensajes y eventos.
- **Subclase SCL07.02.01.03:** Contratos, tiempos de espera y reintentos.

#### Submódulo SM07.03 — Consistencia y coordinación

##### Clase CL07.03.01 — Consistencia y disponibilidad ante fallos
**Referencia anterior:** Clase 7.3 — Razonar sobre consistencia y coordinación entre servicios (unidad dividida; véase tabla de migración).

- **Subclase SCL07.03.01.01:** Consistencia y disponibilidad en contexto de fallos.

##### Clase CL07.03.02 — Coordinación, transacciones, workflows y sagas
**Referencia anterior:** Clase 7.3 — Razonar sobre consistencia y coordinación entre servicios (unidad dividida; véase tabla de migración).

- **Subclase SCL07.03.02.01:** Coordinación, transacciones y workflows.
- **Subclase SCL07.03.02.02:** Sagas y compensaciones.

#### Submódulo SM07.04 — Resiliencia y tolerancia a fallos

*Frontera:* los reintentos, la idempotencia y los circuit breakers se estudian como mecanismos ante fallos de interacción distribuida; la política transversal de disponibilidad, recuperación y operación se trata en el bloque 11.

##### Clase CL07.04.01 — Resiliencia y tolerancia a fallos
**Referencia anterior:** Clase 7.4 — Diseñar para fallos en sistemas distribuidos.

- **Subclase SCL07.04.01.01:** Fallos parciales y aislamiento.
- **Subclase SCL07.04.01.02:** Reintentos, idempotencia y circuit breakers.
- **Subclase SCL07.04.01.03:** Recuperación y degradación controlada.

#### Submódulo SM07.05 — Consecuencias y trade-offs de la distribución

##### Clase CL07.05.01 — Consecuencias y trade-offs de la distribución
**Referencia anterior:** Clase 7.5 — Comparar las consecuencias de los mecanismos de distribución.

- **Subclase SCL07.05.01.01:** Trade-offs entre comunicación síncrona, asíncrona y coordinación.
- **Subclase SCL07.05.01.02:** Consecuencias sobre latencia, consistencia, disponibilidad y complejidad operativa.

---

### Módulo M08 — Estilos arquitectónicos y descomposición

**Alcance:** selección y límites de estilos arquitectónicos y unidades de despliegue. **No incluye:** el estudio profundo de brokers, sagas, consistencia o transacciones distribuidas, que corresponde al bloque 7.

**Competencia principal:** C11. Justificar la forma de descomposición y las unidades de despliegue frente a restricciones del caso.

#### Submódulo SM08.01 — Estilos y estructuras arquitectónicas

##### Clase CL08.01.01 — Capas y monolito modular
**Referencia anterior:** Clase 8.1 — Comparar estilos arquitectónicos (unidad dividida; véase tabla de migración).

- **Subclase SCL08.01.01.01:** Arquitectura en capas.
- **Subclase SCL08.01.01.02:** Monolito y monolito modular.

##### Clase CL08.01.02 — Service-based architecture y SOA
**Referencia anterior:** Clase 8.1 — Comparar estilos arquitectónicos (unidad dividida; véase tabla de migración).

- **Subclase SCL08.01.02.01:** Service-based architecture y SOA.

##### Clase CL08.01.03 — Microservicios
**Referencia anterior:** Clase 8.1 — Comparar estilos arquitectónicos (unidad dividida; véase tabla de migración).

- **Subclase SCL08.01.03.01:** Microservicios.

#### Submódulo SM08.02 — Límites y unidades de despliegue

##### Clase CL08.02.01 — Límites y unidades de despliegue
**Referencia anterior:** Clase 8.2 — Diseñar límites de descomposición.

- **Subclase SCL08.02.01.01:** Límites de módulos, servicios y despliegue.
- **Subclase SCL08.02.01.02:** Acoplamiento estático y dinámico.
- **Subclase SCL08.02.01.03:** Autonomía y tamaño de los componentes.

#### Submódulo SM08.03 — Elegir una estrategia de descomposición

##### Clase CL08.03.01 — Elegir una estrategia de descomposición
**Referencia anterior:** Clase 8.3 — Justificar si conviene mantener, modularizar o distribuir.

- **Subclase SCL08.03.01.01:** Señales de que conviene mantener o modularizar un monolito.
- **Subclase SCL08.03.01.02:** Beneficios y costes de distribuir.
- **Subclase SCL08.03.01.03:** Relación entre límites técnicos y de dominio.

---

### Módulo M09 — APIs como arquitectura

**Alcance:** diseño, especificación, compatibilidad y evolución de contratos de API. **No incluye:** modelado completo de amenazas, identidad y estándares de autorización, que corresponde al bloque 11.

**Competencia principal:** C12. Definir contratos API utilizables, compatibles, protegibles y observables.

#### Submódulo SM09.01 — Contratos y diseño de APIs

##### Clase CL09.01.01 — Contratos y diseño de APIs
**Referencia anterior:** Clase 9.1 — Diseñar un contrato de API.

- **Subclase SCL09.01.01.01:** Contratos, recursos, operaciones y semántica.
- **Subclase SCL09.01.01.02:** Consistencia y usabilidad de una API.
- **Subclase SCL09.01.01.03:** Especificación y documentación.

#### Submódulo SM09.02 — Estilos de API

##### Clase CL09.02.01 — REST como estilo de API
**Referencia anterior:** Clase 9.2 — Comparar estilos de API (unidad dividida; véase tabla de migración).

- **Subclase SCL09.02.01.01:** REST.

##### Clase CL09.02.02 — RPC y GraphQL
**Referencia anterior:** Clase 9.2 — Comparar estilos de API (unidad dividida; véase tabla de migración).

- **Subclase SCL09.02.02.01:** RPC.
- **Subclase SCL09.02.02.02:** GraphQL.

##### Clase CL09.02.03 — Selección contextual del estilo de API
**Referencia anterior:** Clase 9.2 — Comparar estilos de API (unidad dividida; véase tabla de migración).

- **Subclase SCL09.02.03.01:** Selección del estilo según contexto y necesidades.

#### Submódulo SM09.03 — Evolución y compatibilidad

##### Clase CL09.03.01 — Evolución y compatibilidad
**Referencia anterior:** Clase 9.3 — Evolucionar una API sin romper consumidores innecesariamente.

- **Subclase SCL09.03.01.01:**.
- **Subclase SCL09.03.01.02:** Cambios compatibles e incompatibles.
- **Subclase SCL09.03.01.03:** Estrategias de migración de consumidores.

#### Submódulo SM09.04 — Operación y protección del contrato API

*Frontera:* los controles se abordan desde el límite API. El modelado de amenazas, identidad, OAuth 2.0 y OpenID Connect se profundizan en el bloque 11.

##### Clase CL09.04.01 — Protección del contrato y gestión del tráfico API
**Referencia anterior:** Clase 9.4 — Diseñar un contrato API controlable y operable (unidad dividida; véase tabla de migración).

- **Subclase SCL09.04.01.01:** Controles de acceso en la frontera de la API.
- **Subclase SCL09.04.01.02:** Gateways, límites de tráfico y gestión de APIs.

##### Clase CL09.04.02 — Pruebas y observabilidad específica de API
**Referencia anterior:** Clase 9.4 — Diseñar un contrato API controlable y operable (unidad dividida; véase tabla de migración).

- **Subclase SCL09.04.02.01:** Pruebas y observabilidad de APIs.

---

### Módulo M10 — Datos, persistencia y consistencia arquitectónica

**Alcance:** propiedad del dato, modelos de persistencia, transacciones del almacenamiento y patrones de datos. **No incluye:** coordinación de transacciones entre servicios, que corresponde al bloque 7.

**Competencia principal:** C13. Justificar propiedad, persistencia y patrones de datos mediante consistencia, operación y trade-offs.

#### Submódulo SM10.01 — Datos y límites de responsabilidad

##### Clase CL10.01.01 — Datos y límites de responsabilidad
**Referencia anterior:** Clase 10.1 — Asignar responsabilidades y propiedad de los datos.

- **Subclase SCL10.01.01.01:** Ownership de datos.
- **Subclase SCL10.01.01.02:** Persistencia y límites de dominio.
- **Subclase SCL10.01.01.03:** Repositorios y acceso a datos.

#### Submódulo SM10.02 — Modelos y tecnologías de persistencia

##### Clase CL10.02.01 — Modelos y tecnologías de persistencia
**Referencia anterior:** Clase 10.2 — Elegir una estrategia de persistencia por sus drivers.

- **Subclase SCL10.02.01.01:** Necesidades operacionales y analíticas.
- **Subclase SCL10.02.01.02:** Selección de modelos/tecnologías por requisitos.
- **Subclase SCL10.02.01.03:** Costes de acceso, evolución y operación.

#### Submódulo SM10.03 — Transacciones, concurrencia e invariantes de datos

##### Clase CL10.03.01 — Transacciones, concurrencia e invariantes de datos
**Referencia anterior:** Clase 10.3 — Mantener la corrección de los datos dentro de sus límites de persistencia.

- **Subclase SCL10.03.01.01:** Transacciones dentro del límite de almacenamiento.
- **Subclase SCL10.03.01.02:** Consistencia, concurrencia e invariantes de datos.
- **Subclase SCL10.03.01.03:** Proyecciones y modelos de lectura desde la perspectiva de los datos.

#### Submódulo SM10.04 — Patrones de datos y trade-offs

*Frontera:* los efectos de CQRS y event sourcing sobre lectura, escritura y persistencia se estudian aquí; su motivación de dominio puede introducirse en el bloque 6 sin repetir su análisis técnico. La coordinación transaccional entre servicios pertenece al bloque 7.

##### Clase CL10.04.01 — Compartición, replicación y reconstrucción de datos
**Referencia anterior:** Clase 10.4 — Comparar patrones y estrategias de datos mediante sus trade-offs (unidad dividida; véase tabla de migración).

- **Subclase SCL10.04.01.01:** Alternativas para compartir, replicar o reconstruir datos.

##### Clase CL10.04.02 — CQRS y event sourcing como patrones de datos
**Referencia anterior:** Clase 10.4 — Comparar patrones y estrategias de datos mediante sus trade-offs (unidad dividida; véase tabla de migración).

- **Subclase SCL10.04.02.01:** CQRS y event sourcing como patrones de datos: motivación y consecuencias.
- **Subclase SCL10.04.02.02:** Consecuencias sobre acoplamiento, consistencia y disponibilidad.

---

### Módulo M11 — Seguridad, resiliencia, observabilidad y operación

**Alcance:** seguridad transversal, identidad, disponibilidad del servicio, observabilidad y operación segura. **No incluye:** la explicación detallada de fallos parciales, coordinación y semántica de reintentos distribuidos, que corresponde al bloque 7.

**Competencia principal:** C14. Identificar amenazas y fallos transversales y proponer controles, observabilidad y recuperación.

#### Submódulo SM11.01 — Seguridad como preocupación arquitectónica

##### Clase CL11.01.01 — Seguridad como preocupación arquitectónica
**Referencia anterior:** Clase 11.1 — Identificar riesgos de seguridad desde la arquitectura.

- **Subclase SCL11.01.01.01:** Activos, amenazas, vulnerabilidades y riesgos.
- **Subclase SCL11.01.01.02:** Modelado de amenazas.
- **Subclase SCL11.01.01.03:** Seguridad y requisitos arquitectónicos.

#### Submódulo SM11.02 — Identidad y control de acceso

##### Clase CL11.02.01 — Identidad y control de acceso
**Referencia anterior:** Clase 11.2 — Diseñar controles de identidad y acceso.

- **Subclase SCL11.02.01.01:** Autenticación y autorización.
- **Subclase SCL11.02.01.02:** OAuth 2.0 y OpenID Connect.
- **Subclase SCL11.02.01.03:** Límites de confianza y zero trust.

#### Submódulo SM11.03 — Disponibilidad y manejo de fallos

##### Clase CL11.03.01 — Objetivos de disponibilidad y degradación del servicio
**Referencia anterior:** Clase 11.3 — Analizar disponibilidad y recuperación operacional (unidad dividida; véase tabla de migración).

- **Subclase SCL11.03.01.01:** Objetivos de disponibilidad y modos de degradación del servicio.

##### Clase CL11.03.02 — Recuperación, redundancia, errores y atomicidad operativa
**Referencia anterior:** Clase 11.3 — Analizar disponibilidad y recuperación operacional (unidad dividida; véase tabla de migración).

- **Subclase SCL11.03.02.01:** Recuperación, redundancia y resiliencia operacional.
- **Subclase SCL11.03.02.02:** Manejo de errores y atomicidad desde la perspectiva de operación.

#### Submódulo SM11.04 — Observabilidad y operación

##### Clase CL11.04.01 — Observabilidad y operación
**Referencia anterior:** Clase 11.4 — Diseñar observabilidad y operación desde la arquitectura.

- **Subclase SCL11.04.01.01:** Logs, métricas y trazas.
- **Subclase SCL11.04.01.02:** Diagnóstico de comportamiento y fallos.
- **Subclase SCL11.04.01.03:** Releases y operación segura.

---

### Módulo M12 — Cloud, despliegue y arquitectura evolutiva

**Alcance:** decisiones sobre plataforma cloud, despliegue, migración y verificación continua de propiedades arquitectónicas. **No incluye:** enseñar por primera vez seguridad o patrones distribuidos; se aplican conocimientos de los bloques 7 y 11.

**Competencia principal:** C15. Proponer una estrategia cloud/despliegue/evolución con reversibilidad y criterios de verificación.

#### Submódulo SM12.01 — Fundamentos de arquitectura cloud

##### Clase CL12.01.01 — Fundamentos de arquitectura cloud
**Referencia anterior:** Clase 12.1 — Evaluar opciones cloud según los drivers arquitectónicos.

- **Subclase SCL12.01.01.01:** Modelos y mecanismos de cloud relevantes para la arquitectura.
- **Subclase SCL12.01.01.02:** Elasticidad, servicios gestionados y límites operacionales.
- **Subclase SCL12.01.01.03:** Costes y restricciones de operación.

#### Submódulo SM12.02 — Despliegue, releases y migración

##### Clase CL12.02.01 — Despliegue, releases y migración
**Referencia anterior:** Clase 12.2 — Diseñar una estrategia de despliegue o migración.

- **Subclase SCL12.02.01.01:** Despliegue frente a liberación de funcionalidad.
- **Subclase SCL12.02.01.02:** Migración incremental y estrategias de transición.
- **Subclase SCL12.02.01.03:** Riesgos, reversibilidad y criterios de éxito.

#### Submódulo SM12.03 — Evolución y verificación continua

##### Clase CL12.03.01 — Evolución y verificación continua
**Referencia anterior:** Clase 12.3 — Verificar y evolucionar una arquitectura de forma continua.

- **Subclase SCL12.03.01.01:** Fitness functions y verificación de propiedades arquitectónicas.
- **Subclase SCL12.03.01.02:** Automatización de comprobaciones relevantes.
- **Subclase SCL12.03.01.03:** Selección contextual de mecanismos de plataforma, incluido service mesh cuando esté justificado.

---

### Módulo M13 — Arquitectura para AI Engineering

**Alcance:** arquitectura y evaluación de aplicaciones que integran modelos de IA, guiadas por las fuentes disponibles de AI Engineering. **No incluye:** sustituir los fundamentos generales de datos, APIs, seguridad, distribución u operación.

**Competencia principal:** C16. Diseñar una aplicación que integre modelos, datos y sistemas existentes, definiendo evaluación y operación.

#### Submódulo SM13.01 — Fundamentos de AI Engineering

##### Clase CL13.01.01 — Fundamentos de AI Engineering
**Referencia anterior:** Clase 13.1 — Delimitar un problema de software que incorpora AI.

- **Subclase SCL13.01.01.01:** Papel de AI Engineering dentro de la ingeniería de software.
- **Subclase SCL13.01.01.02:** Foundation models y capacidades/limitaciones relevantes.
- **Subclase SCL13.01.01.03:** Selección del caso de uso y expectativas.

#### Submódulo SM13.02 — Arquitectura de aplicaciones basadas en modelos

##### Clase CL13.02.01 — Arquitectura de aplicaciones basadas en modelos
**Referencia anterior:** Clase 13.2 — Identificar componentes y límites de una aplicación AI.

- **Subclase SCL13.02.01.01:** Modelo, datos, aplicación e integración.
- **Subclase SCL13.02.01.02:** Componentes de una aplicación con foundation models.
- **Subclase SCL13.02.01.03:** Integración con APIs y sistemas existentes.

#### Submódulo SM13.03 — Evaluación y calidad de sistemas AI

##### Clase CL13.03.01 — Evaluación y calidad de sistemas AI
**Referencia anterior:** Clase 13.3 — Definir cómo evaluar una aplicación AI.

- **Subclase SCL13.03.01.01:** Estrategias de evaluación.
- **Subclase SCL13.03.01.02:** Calidad, comportamiento esperado e incertidumbre.
- **Subclase SCL13.03.01.03:** Riesgos específicos de sistemas basados en modelos.

#### Submódulo SM13.04 — Operación y evolución de aplicaciones AI

##### Clase CL13.04.01 — Operación y evolución de aplicaciones AI
**Referencia anterior:** Clase 13.4 — Diseñar la arquitectura y operación de una aplicación AI.

- **Subclase SCL13.04.01.01:** Integración, observación y evolución.
- **Subclase SCL13.04.01.02:** Costes, límites y compromisos operativos.

---

### Módulo M14 — Evaluación arquitectónica y análisis económico

**Alcance:** métodos de evaluación, comparación sistemática, evidencia, análisis económico y recomendación. **No incluye:** volver a enseñar el proceso básico de identificación de drivers y alternativas, ya introducido en el bloque 2.

**Competencia principal:** C17. Comparar arquitecturas con evidencia, sensibilidad, costes y riesgos.

#### Submódulo SM14.01 — Evaluación sistemática por escenarios

##### Clase CL14.01.01 — Evaluación sistemática por escenarios
**Referencia anterior:** Clase 14.1 — Evaluar arquitecturas candidatas mediante escenarios y evidencia.

- **Subclase SCL14.01.01.01:** Construir y seleccionar escenarios para evaluar arquitecturas candidatas.
- **Subclase SCL14.01.01.02:** Identificar fortalezas, riesgos y puntos sensibles de las alternativas.
- **Subclase SCL14.01.01.03:** Usar evidencia y experimentación para resolver incertidumbre.

#### Submódulo SM14.02 — Comparación económica de alternativas

##### Clase CL14.02.01 — Comparación económica de alternativas
**Referencia anterior:** Clase 14.2 — Comparar alternativas considerando costes y beneficios.

- **Subclase SCL14.02.01.01:** Costes, beneficios y riesgos.
- **Subclase SCL14.02.01.02:** CBAM y análisis económico arquitectónico.
- **Subclase SCL14.02.01.03:** Sensibilidad de la decisión a supuestos y prioridades.

#### Submódulo SM14.03 — Recomendación arquitectónica

##### Clase CL14.03.01 — Recomendación arquitectónica
**Referencia anterior:** Clase 14.3 — Defender una recomendación arquitectónica con evidencia.

- **Subclase SCL14.03.01.01:** Criterios explícitos y matrices de trade-offs.
- **Subclase SCL14.03.01.02:** Incertidumbre y necesidad de experimentos.
- **Subclase SCL14.03.01.03:** Comunicar recomendación y límites de la evidencia.

---

### Módulo M15 — Práctica profesional del arquitecto

**Alcance:** comunicación profesional, conflicto de intereses, gobernanza, mantenimiento de decisiones e integración final. **No incluye:** sustituir el contenido técnico de los bloques previos.

**Competencia principal:** C18. Comunicar y defender una propuesta integral ante stakeholders, dejando trazabilidad de decisiones y límites de evidencia.

#### Submódulo SM15.01 — Comunicación y documentación

##### Clase CL15.01.01 — Comunicación y documentación
**Referencia anterior:** Clase 15.1 — Comunicar y mantener la documentación arquitectónica.

- **Subclase SCL15.01.01.01:** Adaptar la comunicación a stakeholders técnicos y no técnicos.
- **Subclase SCL15.01.01.02:** Mantener documentación de estructuras, decisiones y consecuencias.
- **Subclase SCL15.01.01.03:** Ciclo de vida, revisión y mantenimiento de ADRs.

#### Submódulo SM15.02 — Stakeholders y organización

##### Clase CL15.02.01 — Stakeholders y organización
**Referencia anterior:** Clase 15.2 — Negociar decisiones arquitectónicas en contexto organizacional.

- **Subclase SCL15.02.01.01:** Preocupaciones, prioridades y conflictos entre stakeholders.
- **Subclase SCL15.02.01.02:** Influencia de la organización en la arquitectura.
- **Subclase SCL15.02.01.03:** Colaboración y toma de decisiones.

#### Submódulo SM15.03 — Gobernanza y evolución arquitectónica

##### Clase CL15.03.01 — Gobernanza y evolución arquitectónica
**Referencia anterior:** Clase 15.3 — Gestionar la evolución arquitectónica con criterio.

- **Subclase SCL15.03.01.01:** Seguimiento de decisiones y consecuencias.
- **Subclase SCL15.03.01.02:** Evolución de la arquitectura y deuda técnica.
- **Subclase SCL15.03.01.03:** Evitar dogmas y soluciones universales.

#### Submódulo SM15.04 — Integración profesional

##### Clase CL15.04.01 — Integración profesional
**Referencia anterior:** Clase 15.4 — Presentar y defender una propuesta arquitectónica integral.

- **Subclase SCL15.04.01.01:** Integrar contexto, drivers, límites, decisiones y consecuencias.
- **Subclase SCL15.04.01.02:** Defender una propuesta ante objeciones y prioridades en conflicto.
- **Subclase SCL15.04.01.03:** Reconocer límites de conocimiento y evidencia pendiente.

---

## 5. Prerrequisitos y progresión

- La tabla de la sección 4 especifica prerrequisitos mínimos observables y resultados esperados por módulo.
- La progresión declarada es **identificar → explicar → justificar → aplicar**.
- Un prerrequisito mínimo no equivale a dominio profundo; las decisiones de avance requieren evidencia alineada al plan de clase.
- Los IDs existentes se conservan; una reorganización visual no autoriza renumeración ni migración automática de progreso.

## 6. Evidencia y evaluación

El índice no registra resultados individuales. Cada plan de clase debe especificar evidencia observable, criterio de evaluación y competencia vinculada. La validación de dominio permanece separada del diseño curricular.

## 7. Limitaciones y condiciones de revisión

- El índice y la matriz orientan la planificación; no aprueban planes, lecturas ni evaluaciones individuales. La matriz de competencias conserva su estado de borrador pendiente de revisión.
- No se infiere dominio del estudiante, asistencia ni progreso por crear una clase o por consultar una fuente. El estado individual se conserva en [COURSE_STATE](../Progress/COURSE_STATE.md) y no se modifica al diseñar clases.
- El currículo no establece una metodología global de tutoría ni proyectos incrementales como secciones autónomas. No inventarlos como política aprobada; si se requieren, especificarlos y evaluarlos en sus artefactos correspondientes.
- Cada plan debe pasar `DRAFT → REVIEW → FIX → RE-CHECK → READY`; una corrección material pendiente impide impartirlo.
- No cambies IDs, jerarquía ni trazabilidad curricular al reformular una clase. Registra límites de evidencia, supuestos y temas fuera de alcance.
