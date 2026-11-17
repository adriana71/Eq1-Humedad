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
| Nombre | Cargo | Organización | Forma de contactar |
|--------|-------|--------------|--------------------|
| Julio Cortés (Productor de tomates) | Junior Grower | Finka Ahuehuetes S.A. de C.V. / Finka, Querétaro | Contacto institucional a través del sitio / administración de Finka Ahuehuetes Querétaro |
|  Montserrat Duarte (Operadora de invernadero | Directora Ejecutiva | Agros Produce LLC, productora de tomates en invernadero en Querétaro, Bajío | A través del canal institucional de la empresa Agros Produce |
| Dra. Rosalinda González Santos (investigadora agricola) | Profesora-Investigadora de tiempo completo / Facultad de Ciencias Naturales, Universidad Autónoma de Querétaro (UAQ) | Universidad Autónoma de Querétaro | Contacto institucional a través del directorio de la Facultad de Ciencias Naturales UAQ. Su perfil público la lista como profesora-investigadora con líneas en agrobiodiversidad y plantas nativas |
| Dr. Irineo Torres Pacheco (Docente de ingenieria) | Docente-Investigador / Facultad de Ingeniería, UAQ - Departamento de Biosistemas, Campus Amazcala | Universidad Autónoma de Querétaro | Contacto institucional a través de la Facultad de Ingeniería UAQ. Aparece como autor en investigación sobre fertilización carbónica en invernaderos y productividad de jitomate en el Campus Amazcala, UAQ | 

## 6. ¿Qué sabemos y qué debemos averiguar?

| Aspecto | Qué sabemos | Qué necesitamos averiguar |
|---------|-------------|---------------------------|
| **Contexto de la situación** | Existe la necesidad de monitorear humedad y temperatura en plántulas de tomate de manera continua y centralizada. | Definir condiciones experimentales precisas: tamaño de macetas, tipo de tierra de cultivo, estados de humedad (0%–100% en intervalos de 10%). |
| **Personas involucradas** | Productores de tomate, operadores de invernaderos, investigadores agrícolas y docentes de ingeniería. | Identificar usuarios finales específicos y sus requerimientos técnicos (ej. nivel de precisión, facilidad de uso, costos). |
| **Cómo se atiende la necesidad** | Actualmente se usan sensores resistivos/capacitivos en contacto directo con la tierra y sistemas manuales de registro. | Diseñar y validar un sensor óptico IR no invasivo, junto con un sistema IoT que registre y visualice datos en tiempo real. |
| **Limitaciones técnicas** | Los sensores tradicionales requieren contacto directo, son más costosos y pueden degradarse con el tiempo. [**Considero que más bien deberían describir cuales son las limitaciones técnicas del sistema propuesto; por ejemplo, ¿solo será obtenido el nivel de humedad de la capa superficial de la tierra en las plantas? o ¿habrá una caracterización para obtener la humedad relativa en el sustrato en función de la reflexión del haz de luz?**]| Determinar sensibilidad del sensor óptico, calibración frente a humedad real, posibles interferencias (luz ambiente, polvo, temperatura). [**¿Cómo podemos caracterizar la humedad del sustrato en función de la humedad de la capa superficial por medio de la reflexión del haz IR?**] |
| **Información técnica necesaria** | Conocemos principios básicos de reflexión de luz IR y funcionamiento de sensores resistivos/capacitivos. | Investigar parámetros ópticos del sustrato, algoritmos de procesamiento de señal, protocolos de comunicación IoT (ej. MQTT, Wi-Fi, LoRa). [**Se debe investigar sobre algoritmos o metodologías de clasificación de la humedad de todo el sustrato en función de la absorción superficial de la luz y quiza alguna otra variable como el peso de la maceta.**] |
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

## 13. Organización documental y estructura del repositorio

### Estructura documental acordada

Para mantener organizada la información y facilitar el seguimiento del desarrollo del proyecto, se estableció una estructura básica para el repositorio de GitHub.

La estructura inicial será la siguiente:

```text
Control-IoT-Invernaderos/
│
├── README.md
│
├── docs/
│   └── expediente-inicial.md
│
└── evidencias/
```

Cada elemento tendrá una función específica:

- **README.md:** presentación general del proyecto. Contendrá una descripción, la oportunidad identificada, los integrantes, sus responsabilidades iniciales, la organización del repositorio y el estado actual del proyecto.
- **docs/:** carpeta destinada a almacenar la documentación formal generada durante las distintas etapas del proyecto.
- **expediente-inicial.md:** documento que contiene la identificación, planeación y organización inicial del proyecto.
- **evidencias/:** carpeta destinada a conservar fotografías, diagramas, capturas de pantalla, resultados experimentales y otros archivos que permitan comprobar los avances realizados.

Esta estructura podrá ampliarse conforme surjan nuevas necesidades durante el desarrollo del proyecto, evitando crear carpetas que todavía no tengan una función definida.

### Regla para nombrar archivos

Como equipo, se establece utilizar nombres descriptivos, breves y consistentes para identificar los archivos incorporados al repositorio.

La regla general será:

**tipo-de-contenido-descripcion-version.extensión**

Se utilizarán las siguientes convenciones:

- Escribir los nombres en minúsculas.
- Utilizar guiones medios (-) para separar las palabras.
- Evitar espacios, acentos y caracteres especiales.
- Utilizar nombres que describan claramente el contenido del archivo.
- Cuando existan distintas versiones de un documento, identificarlas mediante `v01`, `v02`, `v03`, etc.
- Mantener la extensión correspondiente al formato del archivo.

Algunos ejemplos de aplicación serán:

- `expediente-inicial.md`
- `entrevista-productor-01.pdf`
- `diagrama-sensor-optico-v01.png`
- `circuito-acondicionamiento-v02.pdf`
- `prueba-calibracion-humedad-01.csv`
- `fotografia-prototipo-01.jpg`

Esta convención será utilizada por todos los integrantes para facilitar la identificación, consulta y actualización de los archivos.

### Acuerdos de organización y mantenimiento

El equipo acuerda mantener actualizados los documentos del repositorio conforme avance el proyecto.

El responsable de documentación dará seguimiento a la organización y redacción de los archivos, mientras que el administrador de GitHub verificará que los cambios y contribuciones queden registrados correctamente.

Las evidencias del desarrollo se almacenarán en la carpeta correspondiente y los documentos formales se organizarán dentro de `docs/`.

Los cambios realizados deberán registrarse mediante commits con mensajes descriptivos que permitan identificar las modificaciones efectuadas.

## 14. Registro de decisiones iniciales del proyecto

Durante la etapa de planeación, el equipo identificó y estableció diferentes decisiones que orientarán el desarrollo del proyecto. El propósito de este registro es conservar las razones por las cuales se seleccionaron determinadas alternativas y permitir que todos los integrantes puedan consultar los criterios utilizados durante la planeación y las siguientes etapas de desarrollo.

### Decisiones tomadas

**Decisión 1. Desarrollo de un sensor óptico infrarrojo para la medición de humedad**

- **¿Qué se decidió?** Desarrollar y caracterizar un sensor óptico que utilice la reflexión de un haz infrarrojo sobre la superficie del sustrato para estimar su nivel de humedad.
- **¿Por qué se eligió?** Se busca explorar una alternativa de medición menos invasiva que los sensores resistivos o capacitivos tradicionales, los cuales requieren contacto directo con el sustrato.
- **¿Cómo influye en el proyecto?** Define una de las principales líneas de desarrollo e investigación del sistema, por lo que será necesario estudiar las propiedades ópticas del sustrato y la relación entre la luz reflejada y su contenido de humedad.

**Decisión 2. Implementación de un sistema de monitoreo IoT**

- **¿Qué se decidió?** Integrar un sistema IoT para registrar, almacenar y visualizar los datos de humedad y temperatura.
- **¿Por qué se eligió?** Se identificó la necesidad de contar con información continua y centralizada que facilite el seguimiento de las condiciones del cultivo y apoye la toma de decisiones.
- **¿Cómo influye en el proyecto?** Establece la necesidad de desarrollar la comunicación entre los sensores, el microcontrolador y una plataforma que permita consultar los datos obtenidos.

**Decisión 3. Utilizar plántulas de tomate como referencia inicial**

- **¿Qué se decidió?** Tomar las plántulas de tomate como cultivo de referencia para las primeras etapas de experimentación.
- **¿Por qué se eligió?** El equipo identificó el monitoreo de cultivos de tomate en invernaderos como una oportunidad de aplicación del proyecto.
- **¿Cómo influye en el proyecto?** Permite delimitar inicialmente las condiciones de prueba y orientar la investigación hacia las necesidades de este tipo de cultivo, sin descartar que posteriormente el sistema pueda adaptarse a otros cultivos.

**Decisión 4. Utilizar el método gravimétrico como referencia para medir la humedad**

- **¿Qué se decidió?** Utilizar el método gravimétrico para obtener valores de referencia del contenido de agua en el sustrato.
- **¿Por qué se eligió?** Permite comparar las mediciones del sensor óptico con una metodología basada en la diferencia de masa entre una muestra húmeda y una muestra seca.
- **¿Cómo influye en el proyecto?** Servirá como referencia para la caracterización y evaluación experimental del sensor óptico, permitiendo analizar qué tan cercanas son sus mediciones a los valores obtenidos mediante el método gravimétrico.

**Decisión 5. Comparar el sensor óptico con un sensor comercial**

- **¿Qué se decidió?** Realizar comparaciones entre las lecturas del sensor óptico propuesto y las de un sensor comercial de humedad.
- **¿Por qué se eligió?** Se busca evaluar el comportamiento del prototipo y conocer sus diferencias respecto a una alternativa de medición existente.
- **¿Cómo influye en el proyecto?** Permitirá analizar el desempeño del sensor, identificar posibles errores y determinar si requiere ajustes o procedimientos adicionales de calibración.

**Decisión 6. Establecer un objetivo preliminar de precisión**

- **¿Qué se decidió?** Considerar inicialmente un error máximo de ±5 puntos porcentuales de humedad volumétrica como objetivo de desempeño del sensor.
- **¿Por qué se eligió?** Se considera un criterio inicial para orientar el desarrollo y la evaluación del prototipo, tomando en cuenta la utilidad que podría representar para los usuarios.
- **¿Cómo influye en el proyecto?** Servirá como referencia para analizar los resultados experimentales y determinar si el prototipo cumple con los requerimientos planteados. Este objetivo podrá ajustarse de acuerdo con las pruebas realizadas y las necesidades identificadas con los usuarios.

### Criterios para registrar nuevas decisiones

El equipo acuerda documentar las decisiones que definan o modifiquen aspectos importantes del proyecto durante su desarrollo.

Antes de registrar una entrada, se verificará si el equipo seleccionó entre diferentes alternativas o estableció un criterio que influirá en el desarrollo del proyecto. Si se trata únicamente de una actividad o tarea pendiente, no se registrará como decisión.

Cada nueva decisión deberá incluir los siguientes elementos:

- **Decisión tomada:** descripción de la alternativa seleccionada o del criterio establecido.
- **Justificación:** explicación de por qué se eligió esa alternativa y qué aspectos se consideraron.
- **Impacto en el proyecto:** descripción de cómo influye la decisión en el diseño, la investigación, la experimentación o el desarrollo del sistema.

De esta manera, el registro permitirá responder qué eligió el equipo y por qué lo hizo, conservando la justificación de las decisiones y facilitando su consulta durante las diferentes etapas del proyecto.

### 14.3. Actualización del registro

El registro se actualizará conforme se presenten nuevas decisiones durante el desarrollo del proyecto. Cuando una decisión anterior sea modificada, se deberá documentar el cambio y explicar las razones que lo motivaron, evitando perder el contexto de los criterios utilizados inicialmente.

Todos los integrantes podrán proponer nuevas entradas, las cuales deberán revisarse y acordarse en equipo antes de incorporarse al expediente inicial.
