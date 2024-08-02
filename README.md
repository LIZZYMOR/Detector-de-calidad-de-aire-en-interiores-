# Detector de calidad de aire en interiores
Proyecto de Detector de Calidad de aire en interiores, analizado en el Laboratorio de Desarrollos Tecnológicos de la Facultad  de Ciencias Químicas e Ingeniería. 
Este repositorio presenta un proyecto IoT con un prototipo de Detección de aire en interiores, pariendo como aplicación dentro del Laboratorio de DesarrollosTecnológicos (LabDesTec)

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



