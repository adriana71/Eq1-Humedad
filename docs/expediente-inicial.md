# Control IOT de humedad y temperatura en invernaderos.
## 1. Integrantes.
- Barrera Godínez Diego Alejandro 343516
- Mosqueda Ramírez José Manuel 289400
- Párraga Rodríguez Miguel Enrique  314237
- Tamayo Hernández Juan Pablo 313490
## 2. Oportunidad seleccionada.
Desarrolló y caracterización de un sensor óptico de humedad basado en la reflexión de un haz infrarrojo sobre el sustrato, buscando establecer una relación entre la luz reflejada por el sustrato y el nivel de humedad presente.

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
- Investigadores agricolas.
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

# Preguntas para comprensión del Proyecto
1.- ¿Cómo se mide actualmente la humedad de referencia para comparar nuestro sensor?.

2.- ¿Qué precisión mínima necesita el usuario para considerar útil el sensor óptico?.

3.- ¿La luz ambiental afectará la lectura del fotodetector? ¿Se necesita encapsulado oscuro?.

4.- ¿Hay algún cambio si el sensor trabaja dentro de un invernadero? ¿Qué pasa si se usa malla sombra?.

5.- ¿Tenemos balanza de precisión para generar los patrones de humedad?.

6.- ¿El sensor debe funcionar con 5V/3.3V del mismo microcontrolador del Proyecto 2?.

7.- ¿Qué rangos de error han reportado otros sensores ópticos similares?.

# U2.2 — Organizar el equipo para iniciar el proyecto

## Tabla 1: Reconocimiento de Participacion Inicial

| Integrante | Me interesa participar en... | Inicialmente puedo colaborar en... | Me gustaria aprender o desarrollar... |
| :--- | :--- | :--- | :--- |
| @dbarrera13-git |  |  |  |
| @jmosqueda03-ux | Trabajo técnico y planificación en el desarrollo del proyecyo |Planificación y organización del planteamiento y desarrollo | Organización y manejo de nuevas herramientas digitales y de dirección de proyectos |
| @Miguelg30 | Analisis de datos de humedad del suelo y coordinacion del equipo | Organizacion del trabajo, seguimiento de acuerdos y apoyo en GitHub | Liderazgo, manejo de proyectos y trabajo en equipo |
| @JPablo-Tamayo |  |  |  |

## Actividad 2: Necesidades de aprendizaje - Proyecto 3

| Necesidad identificada | Que sabemos actualmente? | Que necesitamos hacer para atenderla? |
| :--- | :--- | :--- |
| Reflexion de haz IR sobre sustrato | Sabemos principios basicos de Fisica e IR | Investigar diseño de emisor-receptor IR y fotodetector |
| Generacion de niveles de humedad patron para caracterizacion | Sabemos que la tierra humeda refleja diferente | Aprender a crear patrones de referencia y validacion cruzada con sensor resistivo/capacitivo |
| Curva de calibracion reflexion vs humedad | Sabemos graficar datos basicos | Aprender Metodos Numericos, regresion no lineal y analisis de repetibilidad y error |

## Definicion de Roles y Responsabilidades (Actividad 3)

| Responsabilidad | Integrante(s) | Rol de Planeacion | Que debera cuidar o verificar? |
| :--- | :--- | :--- | :--- |
| Coordinacion | @Miguelg30 | Coordinador(a) del Equipo | Dar seguimiento a los acuerdos, convocar a reuniones y apoyar en la organizacion del trabajo. |
| Documentacion | @jmosqueda03-ux | Gestor(a) de Documentacion | Mantener actualizado, ordenado y bien redactado el archivo docs/expediente-inicial.md |
| Seguimiento en GitHub | Por definir | Administrador(a) de GitHub | Verificar que los commits y branches esten organizados |

> Comentario de @Miguelg30: Acepto el rol de Coordinador del equipo. Me encargare de dar seguimiento y convocar reuniones.
