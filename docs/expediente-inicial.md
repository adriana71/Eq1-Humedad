# Control IOT de humedad y temperatura en invernaderos.
## 1. Integrantes.
- Barrera Godínez Diego Alejandro 343516
- Mosqueda Ramírez José Manuel 289400
- Párraga Rodríguez Miguel Enrique  314237
- Tamayo Hernández Juan Pablo 313490
## 2. Oportunidad seleccionada.
Desarrollo y caracterización de un sensor óptico de humedad basado en la reflexión de un haz infrarrojo sobre el sustrato, buscando establecer una relación entre la luz reflejada por el sustrato y el nivel de humedad presente.

Creación de un sistema de monitoreo IoT, para registro y visualización de datos, como base para tener una comparativa entre un sensor de humedad tradicional y el sensor óptico propuesto.
## 3. Situación, proceso, necesidad o problemática identificada.
La problemática que identificamos es la falta de un sistema automatizado que permita monitorear de manera individual, continua y centralizada las condiciones de humedad y temperatura de las plántulas de tomate (o cualquier otro cultivo), generando información histórica que facilite la detección de condiciones desfavorables y la toma de decisiones.

Asimismo, identificamos la necesidad de desarrollar un sensor óptico IR para la medición y caracterización de la humedad de una forma menos invasiva y más económica, en comparación con los sensores resistivos o capacitivos, los cuales requieren estar en contacto directo con la tierra.
## 4. Razones por las que consideran pertinente continuar trabajando en ella.
Consideramos que este proyecto es viable, ya que, al estar en una etapa inicial, puede desarrollarse progresivamente a lo largo de los cinco T.D.T.A. que cursaremos durante la ingeniería. Además, nos permitirá aplicar una amplia variedad de los conocimientos y habilidades que iremos adquiriendo a lo largo de nuestra formación.
## 5. Personas, grupos, organizaciones, procesos o sectores que podrían beneficiarse.
Los principales grupos beneficiados que identificamos son:
- Productores de Tomate.
- Operadores de invernaderos.
- Investigadores agrícolas.
- Docentes de ingeniería.
## 6. ¿Qué sabemos y qué debemos averiguar?

| Aspecto | Qué sabemos | Qué necesitamos averiguar |
|---------|-------------|---------------------------|
| **Contexto de la situación** | Existe la necesidad de monitorear humedad y temperatura en plántulas de tomate de manera continua y centralizada. | Definir condiciones experimentales precisas: tamaño de macetas, tipo de tierra de cultivo, estados de humedad (0%–100% en intervalos de 10%). |
| **Personas involucradas** | Productores de tomate, operadores de invernaderos, investigadores agrícolas y docentes de ingeniería. | Identificar usuarios finales específicos y sus requerimientos técnicos (ej. nivel de precisión, facilidad de uso, costos). |
| **Cómo se atiende la necesidad** | Actualmente se usan sensores resistivos/capacitivos en contacto directo con la tierra y sistemas manuales de registro. | Diseñar y validar un sensor óptico IR no invasivo, junto con un sistema IoT que registre y visualice datos en tiempo real. |
| **Limitaciones técnicas** | Los sensores tradicionales requieren contacto directo, son más costosos y pueden degradarse con el tiempo. | Determinar sensibilidad del sensor óptico, calibración frente a humedad real, posibles interferencias (luz ambiente, polvo, temperatura). |
| **Información técnica necesaria** | Conocemos principios básicos de reflexión de luz IR y funcionamiento de sensores resistivos/capacitivos. | Investigar parámetros ópticos del sustrato, algoritmos de procesamiento de señal, protocolos de comunicación IoT (ej. MQTT, Wi-Fi, LoRa). |
| **Aspectos relevantes** | El proyecto puede desarrollarse progresivamente durante la carrera y aplicar múltiples conocimientos adquiridos. | Construir la matriz de pruebas: definir macetas, tierra de cultivo, y niveles de humedad controlados para caracterización experimental. |

# 7. Preguntas para comprensión del Proyecto
1.- ¿Cómo se mide actualmente la humedad de referencia para comparar nuestro sensor?
- Se mide por validación cruzada contra un sensor de humedad de referencia resistivo o capacitivo

2.- ¿Qué precisión mínima necesita el usuario para considerar útil el sensor óptico?
Se requiere una precisión de ±5% de humedad volumétrica.

3.- ¿La luz ambiental afectará la lectura del fotodetector? ¿Se necesita encapsulado oscuro?
- Sí. El sensor mide la intensidad de reflexión de un haz infrarrojo sobre el sustrato, por lo que el fotodetector no distingue entre la radiación emitida y la luz ambiental.

4.- ¿Hay algún cambio si el sensor trabaja dentro de un invernadero? ¿Qué pasa si se usa malla sombra?
- Sí. En invernadero aumentan la temperatura y la humedad ambiental y disminuye la luz directa, lo que modifica la velocidad de secado del sustrato. Con malla sombra disminuye aún más la radiación, lo que reduce la interferencia en el fotodetector, pero también cambia la evaporación.

5.- ¿Tenemos balanza de precisión para generar los patrones de humedad?
- No se hace uso de balanza de precesión en el proyecto.

6.- ¿El sensor debe funcionar con 5V/3.3V del mismo microcontrolador del Proyecto 2?
- Al ser proyectos hermanos el proyecto es necesario que el sensor funcione con los 5V/3.3V del mismo microcontrolador del Proyecto 2.

7.- ¿Qué rangos de error han reportado otros sensores ópticos similares?
- los sensores ópticos y capacitivos de bajo costo reportan errores de ±3% a ±8%, con mayor error en suelo muy seco o saturado, donde la reflectancia se satura.
 
# U2.2 — Organizar el equipo para iniciar el proyecto

## 8. Reconocimiento de Participación Inicial

| Integrante | Me interesa participar en... | Inicialmente puedo colaborar en... | Me gustaría aprender o desarrollar... |
| :--- | :--- | :--- | :--- |
| @dbarrera13-git | Diseño y desarrollo de electrónica | Administración y organización de las tareas e inforacion en GitHub | Liderazgo y administración ágil de desarrollo y coordinación de proyectos |
| @jmosqueda03-ux | Trabajo técnico y planificación en el desarrollo del proyecto |Planificación y organización del planteamiento y desarrollo | Organización y manejo de nuevas herramientas digitales y de dirección de proyectos |
| @Miguelg30 | Análisis de datos de humedad del suelo y coordinación del equipo | Organización del trabajo, seguimiento de acuerdos y apoyo en GitHub | Liderazgo, manejo de proyectos y trabajo en equipo |
| @JPablo-Tamayo |Documentación del proceso de desarrollo del software para el funcionamiento del proyecto|Investigación de los conocimientos y conceptos requeridos para la planeación inicial|Uso de bases de datos para el manejo de plataformas IoT|

## 9. Necesidades de aprendizaje

| Necesidad identificada | ¿Qué sabemos actualmente? | ¿Qué necesitamos hacer para atenderla? |
| :--- | :--- | :--- |
| Reflexión de haz IR sobre sustrato | Sabemos principios básicos de física e IR | Investigar diseño de emisor-receptor IR y fotodetector |
| Generación de niveles de humedad patrón para caracterizacion | Sabemos que la tierra humeda refleja diferente | Aprender a crear patrones de referencia y validación cruzada con sensor resistivo/capacitivo |
| Curva de calibración reflexión vs humedad | Sabemos graficar datos basicos | Aprender métodos numéricos, regresión no lineal y análisis de repetibilidad y error |

## 10. Definición de Roles y Responsabilidades 

| Responsabilidad | Integrante(s) | Rol de Planeación | ¿Qué debera cuidar o verificar? |
| :--- | :--- | :--- | :--- |
| Coordinación | @Miguelg30 | Coordinador del Equipo | Dar seguimiento a los acuerdos, convocar a reuniones y apoyar en la organización del trabajo |
| Documentación | @jmosqueda03-ux | Gestor de Documentación | Mantener actualizado, ordenado y bien redactado el archivo docs/expediente-inicial.md |
| Seguimiento en GitHub | @dbarrera13-git | Administrador de GitHub | Verificar que los commits y branches esten organizados |
| Calidad y recursos | @JPablo-Tamayo | Revisor de calidad | Comprobar el cumplimiento de la checklist de la actividad y consolidar información de investigación  |

## 11. Acuerdos de trabajo

**Canales de comunicación:** De manera oficial y asíncrona se utilizarán los **Issues y Pull Requests de GitHub** para dejar constancia de los avances técnicos, dudas y retroalimentación del proyecto. Para tener una comunicación inmediata entre los miembros se creará un grupo de WhatsApp exclusivo para alertas rápidas, avisos de reuniones y comunicación de emergencias. Para sesiones de trabajo se utilizará como medio de comunicación efectivo una videollamada semanal a través de Microsoft Teams o Zoom, pero primordialmente serán de manera presencial en la universidad, para revisar avances conjuntos.

**Distribución y seguimiento:** Toda actividad se registrará en el **Proyecto de Github** del repositorio, asignando explícitamente un responsable y una fecha límite. El coordinador actualizará el estado de los pendientes en cada sesión semanal, clasificando las tareas en: *Por hacer*, *En proceso* y *Hecho*.

**Fechas y pendientes:** Se respetarán las fechas de entrega establecidas por la profesora, nuestro asesor de proyecto y en conjunto de acuerdo a las necesidades del trabajo. Para evitar retrasos, el equipo entregará sus avances individuales 12 horas antes de la fecha límite oficial del profesor.

**Atención a dificultades o incumplimientos:** Si un integrante no puede cumplir con su tarea por razones de fuerza mayor, deberá avisar al grupo con al menos 24 horas de anticipación. Ante un retraso justificado, el equipo redistribuirá la carga de trabajo para no afectar el cronograma general. En caso de que un integrante no cumpla de forma reiterada y sin justificación, se realizará una llamada de atención en conjunto con el profesor.

**Resolución de diferencias:** Cualquier desacuerdo sobre el diseño, algoritmos o metodologías se resolverá argumentando con bases técnicas y datos de investigación. Si persiste el empate en una decisión de planeación, se realizará una votación por mayoría simple. En caso de un conflicto mayor, el gestor de documentación actuará como mediador neutral.

**Revisión antes de entregar:** Durante la etapa inicial de planeación el uso de múltiples ramas se deja a consideración del editor en base a su criterio de la complejidad de los cambios realizados, si el cambio no puede tener un efecto critico en el proyecto se permite el trabajar directamente sobre el main; en etapas posteriores, una vez iniciado con el desarrolló y ejecución del proyecto será obligatorio trabajar en ramas auxiliares y cada cambio tendrá que ser aceptado por lo menos por otro integrante del equipo dejando documentación clara de los cambios realizados. Estas observaciones también podrán realizarse en las sesiones de reunión del equipo. El gestor de documentación revisará la ortografía, coherencia y formato de los archivos antes de la entrega final.

**Difusión de decisiones:** Las decisiones tomadas en las reuniones verbales se registrarán al final de la sesión en el archivo `docs/expediente-inicial.md` o en el chat oficial. Todo acuerdo que modifique el rumbo del desarrollo quedará documentado de forma pública en el repositorio.

