Desarrollo de un analizador estático inteligente para la evaluación automatizada de controles de seguridad basados en OWASP Top 10:2025 en código fuente Python y JavaScript

Actualmente, muchas vulnerabilidades de seguridad en aplicaciones web se originan durante la etapa de desarrollo debido a prácticas incorrectas de programación, configuraciones inseguras o falta de validación de controles de seguridad. La detección temprana de estos problemas resulta fundamental, ya que corregir vulnerabilidades después del despliegue implica mayores costos económicos, riesgos operativos y exposición de información sensible.
Según OWASP (2025), las aplicaciones modernas continúan presentando riesgos asociados a problemas como control de acceso deficiente, fallos criptográficos, inyección de código, configuraciones inseguras y fallos en la gestión de componentes externos. Estas vulnerabilidades pueden ser introducidas accidentalmente por los desarrolladores debido a desconocimiento, falta de herramientas de revisión o ausencia de procesos automatizados de seguridad durante el ciclo de desarrollo.
Asimismo, herramientas tradicionales de análisis de seguridad como OWASP ZAP, SonarQube, Semgrep y Bearer CLI ofrecen capacidades importantes para identificar vulnerabilidades; sin embargo, muchas requieren configuraciones adicionales, poseen alcances generales o están enfocadas en diferentes etapas del ciclo de desarrollo, lo que puede dificultar su adaptación para una evaluación específica basada en controles del OWASP Top 10:2025.
De acuerdo con OWASP (2025), incorporar mecanismos de seguridad desde las primeras fases del desarrollo permite aplicar el enfoque de Security by Design, reduciendo la probabilidad de introducir vulnerabilidades en el software final.
Por ello, surge la necesidad de desarrollar un sistema de análisis estático que permita evaluar automáticamente el código fuente de proyectos desarrollados en Python y JavaScript, identificando patrones inseguros relacionados con OWASP Top 10:2025, generando resultados cuantificables sobre el nivel de cumplimiento de controles de seguridad y proporcionando recomendaciones de mejora.

Objetivos de investigación
Objetivo general de investigación

Analizar y desarrollar un modelo de evaluación automatizada basado en análisis estático que permita identificar vulnerabilidades y medir el nivel de cumplimiento de controles de seguridad establecidos en OWASP Top 10:2025 para proyectos desarrollados en Python y JavaScript.

Objetivos específicos de investigación
Identificar los principales controles de seguridad definidos en OWASP Top 10:2025 aplicables al análisis estático de código fuente.
Determinar patrones de programación insegura asociados a vulnerabilidades como inyección, fallos criptográficos, configuraciones inseguras y problemas de control de acceso.
Comparar las capacidades y limitaciones de herramientas existentes de análisis estático y dinámico como SonarQube, Semgrep, Bearer CLI y OWASP ZAP.
Definir una metodología de evaluación que permita calcular indicadores de cumplimiento de seguridad por regla, categoría OWASP y proyecto analizado.
Evaluar la precisión del analizador mediante pruebas sobre proyectos con vulnerabilidades conocidas.

Objetivos de solución medibles
Objetivo general de solución
Implementar un analizador estático denominado OWASP Guard, capaz de revisar código fuente Python y JavaScript, detectar malas prácticas de seguridad relacionadas con OWASP Top 10:2025 y generar un reporte cuantitativo del nivel de cumplimiento.

Objetivos específicos de solución
Objetivo	Indicador medible
Implementar un motor de análisis estático para código Python y JavaScript	Analizar correctamente archivos .py y .js
Implementar reglas de detección basadas en OWASP Top 10:2025	Desarrollar mínimo 20 reglas de seguridad
Detectar vulnerabilidades mediante patrones de código inseguro	Identificar al menos 80% de vulnerabilidades introducidas en casos de prueba controlados
Generar reportes de resultados de seguridad	Crear reportes con vulnerabilidad encontrada, severidad, ubicación y recomendación
Calcular nivel de cumplimiento OWASP del proyecto analizado	Mostrar porcentaje global y por categoría OWASP
Diseñar una arquitectura escalable	Permitir agregar nuevas reglas y lenguajes sin modificar el núcleo principal
Evaluar el funcionamiento del sistema	Ejecutar pruebas sobre mínimo 5 proyectos vulnerables y comparar resultados
Variables principales de investigación

Fuentes
OWASP Foundation. (2025). OWASP Top 10:2025 – The Ten Most Critical Web Application Security Risks.
https://owasp.org/www-project-top-ten/
OWASP Foundation. (2021). OWASP Application Security Verification Standard (ASVS).
https://owasp.org/www-project-application-security-verification-standard/
SonarSource. (2025). SonarQube Documentation: Code Quality and Security Analysis.
https://docs.sonarsource.com/
Semgrep. (2025). Semgrep Documentation: Static Application Security Testing.
https://semgrep.dev/docs/
OWASP. (2025). OWASP Zed Attack Proxy (ZAP) Documentation.
https://www.zaproxy.org/docs/
