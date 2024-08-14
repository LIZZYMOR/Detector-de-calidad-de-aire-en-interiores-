# Detector de calidad de aire en interiores-DEAINT
Proyecto de Detector de Calidad de aire en interiores, analizado en el Laboratorio de Desarrollos Tecnológicos de la Facultad  de Ciencias Químicas e Ingeniería. 
Este repositorio presenta un proyecto IoT con un prototipo de Detección de aire en interiores, partiendo como punto de aplicación.

## Introducción
En el contexto de un laboratorio cerrado que utiliza impresion por resina, es fundamental gestionar y minimizar la exposición a los gases nocivos liberados durante el proceso de impresion de piezas en 3D. Este proyecto se centra en la implementación  de un sistema de análisis de datos robusto y continuo para monitorear la calidad del aire y asegurar un entorno de trabajo seguro y saludable.

## Problemática
La contaminación del aire es una mezcla de sustancias peligrosas de origen humano y natural. La contaminación del aire puede aumentar el riesgo de infecciones respiratorias, enfermedades cardiacas, accidentes cerebrovasculares y cancer de pulmón.

Algunas resinas de impresión 3D contienen productos químicos que pueden tener efectos nocivos para la salud, incluido un posible riesgo de cáncer. 

La exposición a largo plazo de ciertos productos químicos presentes en la resina, como los compuestos orgánicos volátiles y los monomeros sin curar, pueden presentar un riesgo para la salud. Estos compuestos pueden liberarse durante el proceso de impresión y generar vapores o partículas que se inhalan o entran en contacto con la piel.

**Niveles de CO2 o Dióxido de Carbono:**
Es un gas incoloro e inodoro que forma parte de la naturaleza y no es realmente un tóxico, pero produce el desplazamiento del oxígeno y en concentraciones altas de más de 300.00 ppm, puede producir asfixia. Es un indicador fundamental para determinar la necesidad de renovacion de aire.

- En ambientes interiores no industriales, los valores usuales de CO2 en el aire estan entre 350 y 450 ppm.
- Para la calidad del aire interiores, se concidera aceptables concentraciones de CO2 entre 600 y 800 ppm.

En laboratorios, se recomienda mantener los niveles por debajo de 5000 ppm para exposiciones diarias de 8 horas. 

## Solución Propuesta 
El prototipo propuesto aborda esta problemática mediante la integración del monitoreo a través de un sensor mq-135 que detecta niveles anormales de CO2 en el aire.
El detector de aire de interiores es manejado principalmente por un microprocesador (Raspberry Pi 4B) que se encarga de ser un servidor, para  recibir datos de el sensor de CO2, sensor de partículas, sensor de polvo y el sensor de gases para la medición del aire en un ambiente determinado, conectandos a un microcontrolador para el intercambio de la información, recopilando los datos en mysql y posterior visualización en Node-RED.

Con la utilización de estos sensores se pueden identificar las zonas o estancias habilitadas en las que los niveles de dióxido de carbono, polvo, partículas y gases son superiores a los aceptables. Los sensores al detectar niveles inadmisibles ajustaran los sistemas de ventilación y el flujo de aire a estas necesidades con el fin de obtener la adecuada renovación y calidad de aire interior, para ello se utilizará una alarma de manera visual y auditiva mediante un led y un buzzer que notificará a los usuarios de evacuar la zona de ser necesario, un extractor y un servo que abrirá las ventanas del laboratorio para mantenerla ventilada.

## Objetivos Específicos
1. Implementar sensores y dispositivos de monitoreo en tiempo real para medir la concentración de gases nocivos liberados duarante el proceso de impresión por resina.
2. Analizar los datos recogidos para identificar tendencias y patrones en la liberación de gases, permitiendo ajustes en la ventilación y el uso de equipos de protección personal (EPP) para minimizar la exposición a estos contaminantes.

## Materiales Necesarios
- ESP32 DEV KIT 1
- Raspberry Pi 4B 8gb
- Sensor MQ-135
- Servomotor SG90
- Led Rojo
- Buzzer
- Ventilador 12V
- 2 Resistencias 220 ohms

## Circuito
![](https://github.com/LIZZYMOR/Detector-de-calidad-de-aire-en-interiores-/blob/main/imagenes/CIRCUITO%20DEAINT.png)

## Servicios
**Registro:** 
Acceso a los datos recopilados para ver en que horarios se encuentra en óptimas condiciones el ambiente de trabajo y cuales son las tareas que perjudican los niveles aceptables para una adecuada calidad de aire.

## Resultados Esperados
Con este proyecto se espera mantener a los estudiantes y/o trabajadores en un ambiente adecuado para que se realicen sus actividades de manera eficiente y cuidando su salud de enfermedades respiratorias a largo plazo por estar en contacto con agentes contaminantes, que forman parte de los compuestos desprendidos por la resina y la estación de soldar.

## Conclusiones
Este proyecto fue elaborado con la finalidad de mantener un análisis de datos dentro de un laboratorio cerrado, en donde constantemente se utiliza la impresión por resina, el cual libera gases a largo plazo, que son nocivos para la salud y este escenario es escalable en la industria, oficinas, laboratorios de alta gama e incluso hogares para salvaguardar la salud de los trabajadores y ofrecer más trabajos dignos y seguros.

Este proyecto fue realizado en el marco del curso IoT Essentials Developer impartido por [Codigo IoT ](https://www.codigoiot.com/) y organizado por la [Asociación Mexicana del Internet de las Cosas](https://www.asociacioniot.org/).












