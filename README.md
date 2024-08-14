# Detector de calidad de aire en interiores
Proyecto de Detector de Calidad de aire en interiores, analizado en el Laboratorio de Desarrollos Tecnológicos de la Facultad  de Ciencias Químicas e Ingeniería. 
Este repositorio presenta un proyecto IoT con un prototipo de Detección de aire en interiores, partiendo como punto de aplicación.

## Introducción
En el contexto de un laboratorio cerrado que utiliza impresion por resina, es fundamental gestionar y minimizar la exposición a los gases nocivos liberados durante el proceso de impresion de piezas en 3D. Este proyecto se centra en la implementacion  de un sistema de analisis de datos robusto y conntinuo para monitorear la calidad del aire y asegurar un entorno de trabajo seguro y saludable.

## Problemática
La contaminación del aire es una mezcla de sustancias peligrosas de origen humano y natural. La contaminación del aire puede aumentar el riesgo de infecciones respiratorias, enfermedades cardiacas, accidentes cerebrovasculares y cancer de pulmon.

Algunas resinas de impresion 3D contienen productos quimicos que pueden tener efectos nocivos para la salud, incluido un posible riesgo de cancer. 

La exposicion a largo plazo de ciertos productos quimicos presentes en la resina, como los compupestos organicos volatiles y los monomeros sin curar, puede presentar un riesgo para la salud. Estos compuestos pueden liberarse durante el proceso de impresion y generar vapores o particulas que se inhalan o entran en contacto con la piel.

**Niveles de CO2 o Dioxido de Carbono:**
Es un gas incoloro e inodoro que forma parte de la naturaleza y no es realmente un toxico, pero produce el desplazamiento del oxigeno y en concentraciones altas de mas de 300.00 ppm, puede producir asfixia. Es un indicador fundamental para determinar la necesidad de renovacion de aire.

- En ambientes interiores no industriales, los valores usuales de CO2 en el aire estan entre 350 y 450 ppm.
- Para la calidad del aire interiores, se concidera aceptables concentraciones de CO2 entre 600 y 800 ppm.

En laboratorios, se recomienda mantener los niveles por debajo de 5000 ppm para exposiciones diarias de 8 horas. 

## Solución Propuesta 
El prototipo propuesto aborda esta problematica mediante la integracion del monitoreo a traves de un sensor mq-135 que detecta niveles anormales de CO2 en el aire.
El detector de aire de interiores es manejado principalmente por un microprocesador (Raspberry Pi 4B) que se encarga de ser un servidor, para  recibir datos de el sensor de CO2, sensor de particulas, sensor de polvo y el sensor de gases para la medicion del aire en un ambiente determinado, conectandos a un microcontrolador para el intercambio de la informacion, recopilando los datos en mysql y posterior visualizacion en NodeRED.

Con la utilizacion de estos sensores se pueden identificar las zonas o estancias habilitadas en las que los niveles de dioxido de carbono, polvo, particulas y gases son superiores a los aceptables. Los sensores al detectar niveles inadmisibles ajustaran los sistemas de ventilacion y el flujo de aire a estas necesidades con el fin de obtener la adecuada renovacion y calidad de aire interior, para ello se utilizará una alarma de manera visual y auditiva mediante un le y un buzzer que notificara a los usuarios de evacuar la zona de ser necesario, un extractor y servo que abrirá las ventanas del laboratorio para mantenerla ventilada.

## Objetivos Especificos
1. Implementar sensores y dispositivos de monitoreo en tiemp real para medir la concentracion de gases nocivos liberados duarante el proceso de impresion por resina.
2. Analizar los datos recogidos ara identificar tendencias y patrones en la liberacion de gases, permitiendo ajustes en la ventilacion y el uso de equipos de proteccion personal (EPP) para minimizar la exposición a estos contaminantes.

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
Acceso a los datos recopilados para ver en que horarios se encuentra en optimas condiciones el ambiente de trabajo y cuales son las tareas que perjudican los niveles aceptables para una adecuada calidad de aire.

## Resultados Esperados
Con este proyecto se espera mantener a los estudiantes y/o trabajadores en un ambiente adecuado para que se realicen sus actividades de manera eficiente y cuidando su salud de enfermedades respiratorias a largo plazo por estar en contacto con agentes contaminantes, que forman parte de kos compuestos desprendidos por la resina y la estacion de soldar.

## Conclusiones
Este proyecto fue elaborado con la finalidad de mantener un analisis de datos dentro de un laboratorio cerrado, en donde constantemente se utiliza la impresión por resina, el cual libera gases a largo plazo, que son nocivos para la salud y este escenario es escalable en la industria, oficinas, laboratorios de alta gama e incluso hogares para salvaguardar la salud de los trabajadores y ofrecer trabajos dignos y seguros.

Este proyecto fue realizado en el marco del curso IoT Essentials Developer impartido por [Codigo IoT ](https://www.codigoiot.com/) y organizado por la [Asociación Mexicana del Internet de las Cosas](https://www.asociacioniot.org/).












