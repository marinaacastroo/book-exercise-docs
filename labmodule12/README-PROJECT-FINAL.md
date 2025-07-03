# Lab Module 12 - Semester Project - Final Write-up

NOTE: Be sure to implement all the Lab Module 12 requirements listed at Lab Module 12.


## Description

Describe your idea in 1 paragraph (at least 2 or 3 sentences).
Mi proyecto consiste en un sistema inteligente para monitorizar el ambiente y controlar la calidad del aire en espacios interiores. Utiliza un dispositivo de borde (CDA) que mide temperatura, humedad y calidad del aire, y un gateway (GDA) que recopila estos datos, toma decisiones localmente y se conecta a la nube para almacenamiento y visualización.



## What - The Problem 

What problem did you tackle and why does it matter? Write 1 to 2 paragraphs in response.
El reto abordado es la falta de sistemas automáticos que permitan detectar y responder a condiciones ambientales desfavorables en interiores, como mala calidad del aire o variaciones bruscas de temperatura y humedad. Este problema es importante porque puede afectar la salud y el confort de las personas, especialmente en lugares cerrados donde la ventilación es limitada.
Contar con un sistema que no solo monitorice, sino que también actúe automáticamente ante situaciones de riesgo, ayuda a prevenir problemas de salud y mejora la calidad de vida en hogares, oficinas o centros educativos.


## Why - Who Cares? 

Why do you care about this particular problem? Write 1 to 2 paragraphs in response.
Me interesa este problema porque la calidad del aire y el ambiente interior suelen ser factores ignorados hasta que generan molestias o problemas de salud. La tecnología IoT permite crear soluciones accesibles y automáticas para monitorizar y actuar en tiempo real, lo que puede marcar una diferencia significativa en el bienestar diario.
Además, este tipo de sistemas es relevante para cualquier persona que pase mucho tiempo en interiores, y demuestra cómo la integración de sensores, lógica local y servicios cloud puede aportar valor real y tangible.


## How - Expected Technical Approach

Write 1 to 2 paragraphs describing the outcomes you achieved.
El sistema desarrollado permite la recolección continua de datos ambientales a través de sensores conectados al CDA. Estos datos se envían al GDA mediante MQTT con TLS, donde se procesan y, si se detectan condiciones adversas, se generan comandos para activar actuadores como un purificador de aire o un LED. Toda la información se transmite a la nube (Ubidots) para su almacenamiento y visualización, y desde la nube también se pueden enviar comandos de actuación al sistema.
La arquitectura modular y el uso de protocolos seguros aseguran la fiabilidad y escalabilidad del sistema, permitiendo su adaptación a diferentes entornos y necesidades.



### System Diagram

Embed a block diagram depicting your overall design, including the CDA, GDA, and Cloud Services interactions.
Be sure to include arrows depicting data flow from one application / service to the next.



Write 1 to 2 paragraphs describing your design.
- CDA → GDA: SensorData (Temperatura, Humedad, Calidad del Aire), SystemPerformanceData (vía MQTT/TLS)
- GDA → CDA: ActuatorData (Comando Purificador, Comando LED) (vía MQTT/TLS)
- GDA → Nube (Ubidots): SensorData y SystemPerformanceData (vía MQTT/TLS)
- Nube (Ubidots) → GDA: ActuatorData (Comando LED) (vía MQTT/TLS))


### What THREE (3) sensors and ONE (1) actuator did you use (add more if you wish)?

- CDA Sensor 1:  Sensor de Temperatura

- CDA Sensor 2: Sensor de Humedad

- CDA Sensor 3: Sensor de Calidad del Aire

- CDA Actuator 1: Actuador Purificador de Aire (además del LED y HVAC existentes)



### What ONE (1) CDA protocol and TWO (2) GDA protocols did you implement (add more if you wish)?

- CDA to GDA Protocol: MQTT (con TLS)

- GDA to CDA Protocol: MQTT (con TLS)

- GDA to Cloud Protocol: MQTT (con TLS)

- Cloud to GDA Protocol: MQTT (con TLS)


 
### What TWO (2) cloud services / capabilities did you use (add more if you wish)?

- Cloud Service 1 (data ingress - all inputs): Ubidots (recepción y almacenamiento de datos)

- Cloud Service 2 (data egress - all actuation events): Ubidots (envío de comandos de actuación)



## Screen Shots Representing Cloud Services



### Screen Shots Representing Visualized Data

NOTE: Include (at least) TWO (2) screen shots - one showing at least 1 hour
of time-series data from the CDA, and one showing an event being triggered
that results in an actuation event sent to your GDA and then to your CDA.



EOF.
