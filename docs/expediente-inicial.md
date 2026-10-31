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
| **Limitaciones técnicas** | Los sensores tradicionales requieren contacto directo, son más costosos y pueden degradarse con el tiempo. [**Considero que más bien deberían describir cuales son las limitaciones técnicas del sistema propuesto; por ejemplo, ¿solo será obtenido el nivel de humedad de la capa superficial de la tierra en las plantas? o ¿habrá una caracterización para obtener la humedad relativa en función de la reflexión del haz de luz?**]| Determinar sensibilidad del sensor óptico, calibración frente a humedad real, posibles interferencias (luz ambiente, polvo, temperatura). |
| **Información técnica necesaria** | Conocemos principios básicos de reflexión de luz IR y funcionamiento de sensores resistivos/capacitivos. | Investigar parámetros ópticos del sustrato, algoritmos de procesamiento de señal, protocolos de comunicación IoT (ej. MQTT, Wi-Fi, LoRa). |
| **Aspectos relevantes** | El proyecto puede desarrollarse progresivamente durante la carrera y aplicar múltiples conocimientos adquiridos. | Construir la matriz de pruebas: definir macetas, tierra de cultivo, y niveles de humedad controlados para caracterización experimental. |

## 7. Preguntas para comprensión del Proyecto.

1.- ¿Cómo se mide actualmente la humedad de referencia para comparar nuestro sensor?
- Se propone utilizar el método gravimétrico, que consiste en pesar una muestra húmeda y seca para determinar su contenido de agua. Sus resultados se compararán con las lecturas del sensor óptico y de un sensor comercial calibrado (Yin et al., 2013).

2.- ¿Qué precisión mínima necesita el usuario para considerar útil el sensor óptico?
- Se establece como objetivo preliminar un error máximo de ±5 puntos porcentuales de humedad volumétrica. Este requisito deberá validarse mediante pruebas experimentales y ajustarse según las necesidades del cultivo.

3.- ¿La luz ambiental afectará la lectura del fotodetector? ¿Se necesita encapsulado oscuro?
- Sí. La iluminación externa puede alterar la señal recibida. Se propone utilizar un encapsulado que reduzca la luz ambiental y evaluar técnicas de compensación para mejorar la estabilidad de las lecturas.

4.- ¿Hay algún cambio si el sensor trabaja dentro de un invernadero? ¿Qué pasa si se usa malla sombra?
- Sí. La temperatura, la humedad ambiental, la ventilación y la radiación modifican el secado del sustrato. Se evaluará el sensor bajo distintas condiciones de iluminación y se registrarán las variables ambientales relevantes.

5.- ¿Tenemos balanza de precisión para generar los patrones de humedad?
- La disponibilidad de una balanza adecuada y de un horno de secado está pendiente de confirmación. Si no se cuenta con ellos, se solicitará apoyo de un laboratorio para realizar las mediciones gravimétricas de referencia.

6.- ¿El sensor debe funcionar con 5V/3.3V del mismo microcontrolador del Proyecto 2?
- Se busca compatibilidad con la alimentación del microcontrolador compartido. Se deberán confirmar sus niveles de voltaje y verificar los requisitos eléctricos de los componentes mediante sus hojas de datos.

7.- ¿Qué rangos de error han reportado otros sensores ópticos similares?
- Los errores varían según el tipo de suelo, la longitud de onda y la calibración. Yin et al. (2013) reportaron un RMSE de 2.47 % para un modelo no lineal y de 4.75 % para uno lineal en muestras de suelo negro. Estos resultados no son generalizables a cualquier sensor. Por ello, se comparará el prototipo con una referencia gravimétrica y se calculará su error experimental.

## 8. Reconocimiento de Participación Inicial.

| Integrante | Me interesa participar en... | Inicialmente puedo colaborar en... | Me gustaría aprender o desarrollar... |
| :--- | :--- | :--- | :--- |
| @dbarrera13-git | Diseño CAD y desarrollo de electrónica | Administración y organización de las tareas e inforación en GitHub | Liderazgo y administración ágil de desarrollo y coordinación de proyectos |
| @jmosqueda03-ux | Trabajo técnico y planificación en el desarrollo del proyecto |Planificación y organización del planteamiento y desarrollo | Organización y manejo de nuevas herramientas digitales y de dirección de proyectos |
| @Miguelg30 | Análisis de datos de humedad del suelo y coordinación del equipo | Organización del trabajo, seguimiento de acuerdos y apoyo en GitHub | Liderazgo, manejo de proyectos y trabajo en equipo |
| @JPablo-Tamayo |Documentación del proceso de desarrollo del software para el funcionamiento del proyecto|Investigación de los conocimientos y conceptos requeridos para la planeación inicial|Uso de bases de datos para el manejo de plataformas IoT|

## 9. Necesidades de aprendizaje.
| Tema | Conocimientos previos | Conocimientos por adquirir | Recurso de aprendizaje | Aplicación en el proyecto | 
| :--- | :--- | :--- | :--- | :--- |
| Programación en C++ | Fundamentos de programación, variables y estructuras de control. | Lectura de sensores, procesamiento de datos y comunicación serial. | Visual studio / Arduino IDE | Programación de sensores IR y procesamiento de mediciones.|
| Programación de microcontroladores PIC | Conceptos básicos de programación y electrónica digital. | Configuración de puertos, temporizadores, entradas y salidas, y lectura de sensores. | PIC C Compiler | Programación del microcontrolador para adquirir y procesar datos de temperatura y humedad. |
| Diseño de circuitos | Fundamentos de electricidad, componentes electrónicos y diagramas eléctricos. | Simulación de circuitos, selección de componentes y comprobación de conexiones. | Proteus | Simulación y validación del circuito electrónico antes de construirlo. |
| Diseño de PCBs | Conocimientos básicos de circuitos electrónicos. | Diseño esquemático, selección de huellas, distribución de componentes y trazado de pistas. | FUSION 360 (Electronics) | Diseño de la tarjeta electrónica para integrar el microcontrolador y los sensores. |
| Manufactura de PCBs | Conocimientos básicos de electrónica y soldadura. | Generación de archivos Gerber, preparación de archivos de fabricación, perforación y montaje de componentes. | PCB toolkit | Fabricación y ensamblaje de la tarjeta electrónica del sistema. |
| Integración y validación | Conocimientos básicos de electrónica, programación y uso de instrumentos de medición. | Integración de hardware y software, calibración, detección de fallas y comparación con instrumentos de referencia. | Multímetro, data sheets y manuales técnicos | Comprobar que el sistema mida correctamente la temperatura y humedad del cultivo. |
| Diseño CAD | Conocimientos básicos de dibujo técnico y modelado tridimensional. | Diseño de soportes, carcasas y piezas para montaje, considerando dimensiones y accesibilidad. | SOLIDWORKS | Diseñar la carcasa y los soportes para proteger y fijar los componentes del sistema de monitoreo. |

| Integrante | Rol principal | Responsabilidades asignadas | Temas de aprendizaje relacionados |
| :--- | :--- | :--- | :--- |
| @dbarrera13-git | Responsable de electrónica y diseño CAD | Diseñar los circuitos electrónicos, desarrollar la PCB y diseñar los soportes y la carcasa del sistema. Organizar las tareas y los archivos técnicos en GitHub. | Diseño de circuitos, diseño de PCB, manufactura de PCB y diseño CAD. |
| @jmosqueda03-ux | Responsable de planificación e integración del sistema | Organizar las etapas de desarrollo, coordinar la integración del hardware y software, dar seguimiento al cronograma y apoyar en las pruebas del prototipo. | Programación de microcontroladores, integración y validación. |
| @Miguelg30 | Responsable de análisis de datos y seguimiento del proyecto | Analizar las mediciones de humedad y temperatura, organizar el trabajo del equipo, dar seguimiento a los acuerdos y apoyar en la administración de tareas en GitHub. | Adquisición y procesamiento de datos, integración y validación. |
| @JPablo-Tamayo | Responsable de documentación y gestión de datos | Documentar el desarrollo del software, investigar los conceptos requeridos para el proyecto y estudiar las bases de datos y plataformas IoT para almacenar y consultar las mediciones. | Programación en C++, comunicación de datos, almacenamiento y plataformas IoT. |

## 10. Definición de Roles y Responsabilidades.

| Responsabilidad | Integrante(s) | Rol de Planeación | ¿Qué deberá cuidar o verificar? |
| :--- | :--- | :--- | :--- |
| Coordinación | @Miguelg30 | Coordinador del Equipo | Dar seguimiento a los acuerdos, convocar a reuniones y apoyar en la organización del trabajo |
| Documentación | @jmosqueda03-ux | Gestor de Documentación | Mantener actualizado, ordenado y bien redactado el archivo docs/expediente-inicial.md |
| Seguimiento en GitHub | @dbarrera13-git | Administrador de GitHub | Verificar que los commits y branches esten organizados |
| Calidad y recursos | @JPablo-Tamayo | Revisor de calidad | Comprobar el cumplimiento de la checklist de la actividad y consolidar información de investigación  |

## 11. Acuerdos de trabajo.

**Canales de comunicación:** De manera oficial y asíncrona se utilizarán los **Issues y Pull Requests de GitHub** para dejar constancia de los avances técnicos, dudas y retroalimentación del proyecto. Para tener una comunicación inmediata entre los miembros se creará un grupo de WhatsApp exclusivo para alertas rápidas, avisos de reuniones y comunicación de emergencias. Para sesiones de trabajo se utilizará como medio de comunicación efectivo una videollamada semanal a través de Microsoft Teams o Zoom, pero primordialmente serán de manera presencial en la universidad, para revisar avances conjuntos.

**Distribución y seguimiento:** Toda actividad se registrará en el **Proyecto de GitHub** del repositorio, asignando explícitamente un responsable y una fecha límite. El coordinador actualizará el estado de los pendientes en cada sesión semanal, clasificando las tareas en: *Por hacer*, *En proceso* y *Hecho*.

**Fechas y pendientes:** Se respetarán las fechas de entrega establecidas por la profesora, nuestro asesor de proyecto y en conjunto de acuerdo a las necesidades del trabajo. Para evitar retrasos, el equipo entregará sus avances individuales 12 horas antes de la fecha límite oficial del profesor.

**Atención a dificultades o incumplimientos:** Si un integrante no puede cumplir con su tarea por razones de fuerza mayor, deberá avisar al grupo con al menos 24 horas de anticipación. Ante un retraso justificado, el equipo redistribuirá la carga de trabajo para no afectar el cronograma general. En caso de que un integrante no cumpla de forma reiterada y sin justificación, se realizará una llamada de atención en conjunto con el profesor.

**Resolución de diferencias:** Cualquier desacuerdo sobre el diseño, algoritmos o metodologías se resolverá argumentando con base técnica o fundamentos técnicos y datos de investigación. Si persiste el empate en una decisión de planeación, se realizará una votación por mayoría simple. En caso de un conflicto mayor, el gestor de documentación actuará como mediador neutral.

**Revisión antes de entregar:** Durante la etapa inicial de planeación el uso de múltiples ramas se deja a consideración del editor en base a su criterio de la complejidad de los cambios realizados, si el cambio no puede tener un efecto critico en el proyecto se permite el trabajar directamente sobre el main; en etapas posteriores, una vez iniciado con el desarrolló y ejecución del proyecto será obligatorio trabajar en ramas auxiliares y cada cambio tendrá que ser aceptado por lo menos por otro integrante del equipo dejando documentación clara de los cambios realizados. Estas observaciones también podrán realizarse en las sesiones de reunión del equipo. El gestor de documentación revisará la ortografía, coherencia y formato de los archivos antes de la entrega final.

**Difusión de decisiones:** Las decisiones tomadas en las reuniones verbales se registrarán al final de la sesión en el archivo `docs/expediente-inicial.md` o en el chat oficial. Todo acuerdo que modifique el rumbo del desarrollo quedará documentado de forma pública en el repositorio.

## 12. Referencias.

1.- Federlein, J. (2017). New ISA guidelines for managing a calibration program. InTech, International Society of Automation. https://www.isa.org/intech-home/2017/september-october/departments/new-isa-guidelines-for-managing-a-calibration-prog

2.- Yin, Z., Lei, T., Yan, Q., Chen, Z., & Dong, Y. (2013). A near-infrared reflectance sensor for soil surface moisture measurement. Computers and Electronics in Agriculture, 99, 101–107. https://doi.org/10.1016/j.compag.2013.08.029

3.- Yin, Z., Lei, T., Chen, Z., Yan, Q., & Dong, Y. (2013). Comparison of two prediction models for surface soil moisture measurement using near-infrared sensor. 2013 Kansas City, Missouri, July 21–24, 2013. https://doi.org/10.13031/aim.20131596930

4.- A temperature compensated soil specific calibration approach for frequency domain soil moisture sensors for in-situ agricultural applications. (2021). En 2021 IEEE Sensors Applications Symposium (SAS). https://doi.org/10.1109/SAS51076.2021.9530177

5.- Mane, S., Das, N., Singh, G., Cosh, M., & Dong, Y. (2024). Advancements in dielectric soil moisture sensor calibration: A comprehensive review of methods and techniques. Computers and Electronics in Agriculture, 218, Article 108686. https://doi.org/10.1016/j.compag.2024.108686
