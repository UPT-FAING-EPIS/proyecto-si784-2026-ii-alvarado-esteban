OWASP Guard: Sistema inteligente para el análisis y evaluación automatizada de prácticas de seguridad en código fuente

Actualmente, el desarrollo de aplicaciones de software enfrenta el riesgo de incorporar vulnerabilidades de seguridad desde las propias etapas de programación. Estas pueden originarse por prácticas inadecuadas como la falta de controles de acceso, manejo inseguro de información, errores en la autenticación, inyecciones, configuraciones inseguras y otras debilidades presentes en el código fuente.
El OWASP Top 10 constituye una referencia ampliamente utilizada para identificar los riesgos de seguridad más importantes en aplicaciones web. En su edición 2021, OWASP contempla categorías como pérdida de control de acceso, fallas criptográficas, inyección, diseño inseguro, configuración de seguridad incorrecta, componentes vulnerables y desactualizados, fallas de identificación y autenticación, entre otras.
Uno de los problemas es que la identificación de estas deficiencias puede requerir una revisión detallada del código fuente. OWASP señala que la revisión de código permite identificar problemas de seguridad que pueden ser difíciles de encontrar mediante otras técnicas de análisis. Además, la revisión segura requiere analizar aspectos como la lógica de la aplicación, el flujo de datos y los detalles de implementación, actividades que pueden demandar tiempo y conocimientos especializados.
Por otro lado, OWASP recomienda utilizar su Top 10 como una referencia o línea base para iniciar actividades de seguridad de aplicaciones, pero reconoce que no constituye por sí solo un programa completo de seguridad. Esto evidencia la necesidad de contar con mecanismos complementarios que permitan aplicar determinadas prácticas de seguridad de forma sistemática y repetible durante la revisión del código.
Ante esta situación, se propone desarrollar OWASP Guard, un sistema que permita cargar un proyecto o código fuente y realizar un análisis automatizado mediante 10 reglas de seguridad basadas en prácticas y categorías del OWASP Top 10. El sistema identificará los problemas encontrados indicando el archivo y la línea afectada, clasificará cada hallazgo según su nivel de riesgo, explicará el problema y proporcionará una recomendación para su corrección.
Además, OWASP Guard generará un Security Score de 0 a 100 y un dashboard con información resumida sobre el estado de seguridad del proyecto. De esta manera, la herramienta permitirá transformar los resultados del análisis en información comprensible y medible, facilitando la identificación y priorización de problemas de seguridad en el código fuente.

Objetivos de investigación y solución medibles

Objetivo general:
- Desarrollar OWASP Guard, un sistema inteligente capaz de analizar automáticamente código fuente y evaluar su cumplimiento respecto a un conjunto definido de prácticas de seguridad basadas en OWASP, proporcionando detección, clasificación, explicación y recomendaciones de solución de los problemas encontrados.

Objetivos específicos:
- Implementar 10 reglas automatizadas de análisis de seguridad basadas en categorías y prácticas del OWASP Top 10, verificando que cada regla pueda identificar un patrón de código asociado con una práctica insegura.
- Detectar los problemas de seguridad indicando el archivo y la línea de código afectada, logrando que el sistema proporcione una ubicación específica para cada hallazgo identificado.
- Clasificar automáticamente los hallazgos en cuatro niveles de riesgo —crítico, alto, medio y bajo— de acuerdo con criterios definidos para el proyecto.
- Generar una explicación para el 100 % de los hallazgos detectados, indicando qué práctica de seguridad se incumple y por qué representa un riesgo.
- Proporcionar recomendaciones de solución para el 100 % de las reglas implementadas, orientadas a corregir las prácticas inseguras identificadas.
- Implementar un Security Score de 0 a 100 que permita representar cuantitativamente el nivel de cumplimiento de seguridad de cada proyecto analizado.
- Desarrollar un dashboard de resultados que muestre como mínimo la puntuación de seguridad, cantidad de problemas por nivel de riesgo, archivos analizados y reglas incumplidas.
- Evaluar la efectividad del sistema utilizando proyectos de prueba con vulnerabilidades conocidas, calculando el porcentaje de vulnerabilidades detectadas por OWASP Guard.
