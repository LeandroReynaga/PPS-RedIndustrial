# PPS - Red Industrial
## Universidad Nacional de Lomas de Zamora
📍 **Saint-Gobain, Weber Tortuguitas, Argentina**  
👨‍🎓 **Alumno:** Leandro Joel Reynaga Ríos  
📅 **Año:** 2025  

---

## Índice
1. [Introducción](#1-introducción)  
2. [Objetivo](#2-objetivo)  
3. [Descripción del Proyecto](#3-descripción-del-proyecto)  
   3.1 [Investigación inicial](#31-investigación-inicial)  
   3.2 [Definición de alcance](#32-definición-de-alcance)  
   3.3 [Relevamiento de equipos](#33-relevamiento-de-equipos)  
   3.4 [Documentación de ingeniería](#34-desarrollo-de-documentación-de-ingeniería)  
      3.4.1 [Arquitectura de red actual](#341-arquitectura-de-red-actual)  
      3.4.2 [Arquitectura de red futura](#342-arquitectura-de-red-futura)  
      3.4.3 [Listado de direcciones IP](#343-listado-de-direcciones-ip-futura)  
      3.4.4 [Plano Topográfico](#344-plano-topográfico-de-rack01-industrial)  
      3.4.5 [Plano Multifilar](#345-plano-multifilar-de-rack01-industrial)  
      3.4.6 [Plano Unifilar](#346-plano-unifilar-de-rack01-industrial)  
4. [Conclusiones](#4-conclusiones)

---

## 1. Introducción
El presente informe describe la Práctica Profesional Supervisada (PPS) realizada en Saint-Gobain, Weber Tortuguitas, Argentina, como parte de la carrera de Ingeniería Mecatrónica de la Universidad Nacional de Lomas de Zamora (UNLZ).

Como se podrá ver a continuación, en el marco del roadmap de mejora de Infraestructura dentro del área de Industria 4.0, el desarrollo de una red industrial constituye el punto de partida para la implementación de un SCADA centralizado.  

<p align="center">
  <img width="829" height="476" alt="Roadmap Infraestructura" src="https://github.com/user-attachments/assets/193362ba-f207-4f88-b8ba-6028dc1132da" />
  <br>
  <em>Figura 1: Roadmap Infraestructura I4.0 </em>
</p>

### Beneficios y ventajas más importantes  
- Transferencia e intercambio de datos por medio de protocolos de comunicación.  
- Intercambio de datos entre diferentes sectores del proceso y departamentos.  
- Control del proceso operativo desde el área de gestión.  
- Programación a distancia.  
- Visualización de datos en tiempo real.  
- Flexibilidad de implementación de diferentes marcas por medio de protocolos de comunicación.  

Estos beneficios constituyen la base para la escalabilidad hacia entornos de Industria 4.0, posibilitando la convergencia entre IT (Information Technology) y OT (Operational Technology). 

---

## 2. Objetivo  
El objetivo de este proyecto fue realizar la ingeniería correspondiente, aplicando buenas prácticas de diseño y cumpliendo con las normativas establecidas por la empresa, a fin de garantizar una infraestructura de red robusta, segura y escalable.

---

## 3. Descripción del Proyecto  
### 3.1 Investigación inicial  
El proyecto comenzó con una etapa de investigación orientada a comprender la normativa interna de Saint-Gobain y los lineamientos de infraestructura aplicables a redes industriales. Durante esta primera instancia se logró establecer una base sólida de criterios técnicos y de buenas prácticas que permitieron guiar el desarrollo.

<p align="center">
  <img width="1511" height="749" alt="STD SG PPC ARG Red Industrial" src="https://github.com/user-attachments/assets/61c546f3-c336-4879-971d-be72db1ed15b" />
  <br>
  <em>Figura 2: STD SG PPC ARG Red Industrial </em>
</p>

### 3.2 Definición de alcance  
Posteriormente, se llevaron a cabo reuniones con el equipo de planta, en las cuales se relevaron necesidades, problemáticas y expectativas relacionadas con la conectividad y la comunicación de los equipos de producción. Estas instancias de intercambio fueron fundamentales para definir de manera conjunta el alcance del proyecto, estableciendo qué áreas y dispositivos serían incluidos en el estudio.

### 3.3 Relevamiento de equipos    
Con el alcance definido, se realizó un relevamiento de los equipos instalados en la planta. Este trabajo incluyó la identificación de protocolos de comunicación en uso, direcciones IP asignadas y disponibilidad de placas de comunicación en los distintos PLCs y dispositivos. La información obtenida se consolidó en un repositorio técnico que sirvió luego para la etapa de diseño

### 3.4 Desarrollo de documentación de ingeniería    
A partir de este relevamiento, se desarrolló la documentación de ingeniería necesaria para el proyecto. Esto incluye la representación de:  

#### 3.4.1 Arquitectura de red actual
<p align="center">
  <img width="2320" height="1620" alt="Etapa_0 - Arquitectura de Red Actual" src="https://github.com/user-attachments/assets/3c199051-abe6-4979-b282-0a7e5f31990d" />
  <br>
  <em>Figura 3: Etapa 0 - Arquitectura de Red Actual </em>
</p>

A partir del relevamiento realizado en planta se desarrolló la arquitectura de red actual, con el objetivo de conocer la situación inicial sobre la cual se planificará la futura infraestructura.   
Durante este análisis se identificó la necesidad de:  
- Incorporar placas de comunicación en determinados PLC para garantizar la conectividad.
- Realizar un tendido de cableado estructurado acorde a la normativa vigente, utilizando canalizaciones independientes para asegurar orden y la seguridad de la red.
- Implementar un rack en la sala de control, que funcionará como nodo de conexión principal de la línea de producción.
- Instalar dos switches industriales: uno en el rack de la sala de control y otro en el data room, lo que permitirá en una etapa posterior realizar la interconexión entre los entornos IT (Information Technology) y OT (Operational Technology).

#### 3.4.2 Arquitectura de red futura
<p align="center">
  <img width="2320" height="1620" alt="Etapa_1 - Arquitectura de Red Futura" src="https://github.com/user-attachments/assets/64c7ea1b-8b70-4995-afcb-47c40c604508" />
  <br>
  <em>Figura 4: Etapa 1 - Arquitectura de Red Futura </em>
</p>

La propuesta de arquitectura de red futura tiene como finalidad establecer una infraestructura robusta, segura y escalable.  
El diseño contempla los siguientes lineamientos principales:  
- Instalación de racks industriales conectados a sistemas de alimentación segura, garantizando continuidad operativa y protección de los equipos críticos.
- Incorporación de switches industriales SCALANCE, interconectados mediante enlaces de fibra óptica, preparados para asegurar la comunicación a nivel de planta y para la futura interconexión IT/OT.
- Reserva y estandarización de rangos de direcciones IP, facilitando la administración de equipos actuales y la escalabilidad futura.
- Preparación de la infraestructura para la incorporación de un SCADA centralizado, que permita la supervisión y control remoto de los procesos.  

#### 3.4.3 Listado de direcciones IP futura  
<p align="center">
  <img width="1481" height="797" alt="Listado de direcciones IP futura" src="https://github.com/user-attachments/assets/d825cc14-d948-4641-8392-9fc044bd188e" />
  <br>
  <em>Figura 5: Listado de direcciones IP futura </em>
</p>
Este listado detalla las direcciones IP asignadas a los distintos dispositivos de la red industrial, con el objetivo de estandarizar la asignación y facilitar la administración, mantenimiento y escalabilidad de la red.  

#### 3.4.4 Plano Topográfico de Rack01 industrial   
<p align="center">
  <img width="2482" height="1755" alt="(TOR) Topográfico - Rack  01 _rev1" src="https://github.com/user-attachments/assets/95a421aa-32f9-4179-b37f-8d0d0c1fa024" />
  <br>
  <em>Figura 6: (TOR) Topográfico - Rack [01] </em>
</p>

#### Componentes del Rack  
<div align="center">

| Imagen | Descripción |
|--------|-------------|
| <p align="center"><img width="77" height="59" alt="image" src="https://github.com/user-attachments/assets/561573c2-450a-463e-a04e-c23e15e109b5" /> | Bandeja Fibra (FURUKAWA, 35260163) |
| <p align="center"><img width="145" height="47" alt="image" src="https://github.com/user-attachments/assets/614ccc55-22eb-4639-88e5-2b717999fbbe" /> | Organizador de Cable 1u (FAYSER) |
| <p align="center"><img width="124" height="59" alt="image" src="https://github.com/user-attachments/assets/e8419b44-9841-4427-a5a9-6eee809dec39" /> | Patchera Datos 24P (FURUKAWA) |
| <p align="center"><img width="163" height="59" alt="image" src="https://github.com/user-attachments/assets/b4ac3776-3d29-43df-9239-547b7dfd72f4" /> | Switch Industrial XR324 (SIEMENS, 6GK5324-4QG10-3AR2) |
| <p align="center"><img width="92" height="53" alt="image" src="https://github.com/user-attachments/assets/999e6325-465b-42c3-8759-ce73d23a6d50" /> | Patch Cord F/UTP CAT 6A de 4 pares |
| <p align="center"><img width="80" height="59" alt="image" src="https://github.com/user-attachments/assets/4bb10e1e-7d23-4915-9858-3cdb301c2f38" /> | Patch Cord FO (OM4) SC |
| <p align="center"><img width="83" height="47" alt="image" src="https://github.com/user-attachments/assets/da168269-b851-4025-9e2b-1ad41c0153bd" /> | Plug RJ45 macho para armado en campo CAT 6A |
| <p align="center"><img width="63" height="59" alt="image" src="https://github.com/user-attachments/assets/abca83a8-7f8c-4862-b325-749c66e53fca" /> | Jacks RJ45 hembra CAT 6A |
| <p align="center"><img width="85" height="59" alt="image" src="https://github.com/user-attachments/assets/685357ce-5f4e-47cd-92a7-bb440dcdde39" /> | Modulo conector Ethernet |
| <p align="center"><img width="87" height="53" alt="image" src="https://github.com/user-attachments/assets/0027ce27-8e62-4c08-bb00-1d9ad9fb5345" /> | Modulo conector FO |
| <p align="center"><img width="35" height="59" alt="image" src="https://github.com/user-attachments/assets/1dc479e6-803f-4fa4-b37f-2d28d932a569" /> | Interruptor diferencial 25A (SCHNEIDER) |
| <p align="center"><img width="131" height="59" alt="image" src="https://github.com/user-attachments/assets/96abfef5-c043-4afe-8a55-b8f38d727c75" /> | Interruptor termomagnético 20-16-10-6 [A] (SCHNEIDER) |
| <p align="center"><img width="69" height="59" alt="image" src="https://github.com/user-attachments/assets/2777410d-ebb2-4c6a-b871-4314adf06486" /> | Interruptor Conmutador de 3 posiciones (ZOLADA) |
| <p align="center"><img width="103" height="59" alt="image" src="https://github.com/user-attachments/assets/a7846ff5-f328-4097-a8bb-5a6a869b9439" /> | Accesorios de conexión (ZOLADA) |
| <p align="center"><img width="171" height="59" alt="image" src="https://github.com/user-attachments/assets/47138d61-e342-41d3-ad4c-5bc6c64b5d9c" /> | Base Riel Din + Modulo de tomas 220v (CAMBRE) |
| <p align="center"><img width="188" height="59" alt="image" src="https://github.com/user-attachments/assets/fc7a6ed5-2611-4963-83c5-fe3b9ce3e6b5" /> | PDU, Unidad de distribución de energía |
| <p align="center"><img width="171" height="47" alt="image" src="https://github.com/user-attachments/assets/883f3013-5560-4b29-ae95-9b6ba1401d71" /> | UPS 2.2kVA (APC SCHNEIDER, SRT2200RMXLI-NC) |
</div>

<p align="center">
  <img width="449" height="565" alt="image" src="https://github.com/user-attachments/assets/c82d99e2-8203-4548-9b5a-19f2ea6dc1c2" />
  <br>
  <em>Figura 7: Rack [01] </em>
</p>

#### 3.4.5 Plano Multifilar de Rack01 industrial  
<p align="center">
  <img width="2482" height="1755" alt="(TOR) Multifilar de Rack" src="https://github.com/user-attachments/assets/efcd2b53-b9b5-4bb0-afc3-8704dbc2a0dc" />
  <br>
  <em>Figura 8: Plano Multifilar de Rack01 industrial </em>
</p>

El plano multifilar elaborado para el rack industrial refleja la distribución de protecciones, garantizando que cada circuito esté correctamente dimensionado en relación con la carga prevista y a la sección de los conductores instalados.  
Para esta instalación se emplearon conductores de 2,5 mm² de cobre, cuya capacidad de corriente es de aproximadamente 21 A, de acuerdo con las tablas del fabricante. Por este motivo, la protección general del rack se definió con un interruptor termomagnético bipolar de 20 A, asegurando que en ningún caso la corriente supere la capacidad admisible del cableado.  

En cuanto a los consumos individuales:  
- Switch industrial (SW): con un consumo máximo de 1 A, se lo protege con una térmica de 6 A, valor más que suficiente para cubrir la carga sin sobredimensionar la protección.
- PDU (canal de tensión/tomas de servicio): diseñada para admitir hasta 2200 W, se seleccionó una térmica de 10 A, equivalente a unos 2200 W a 220 V.
- UPS: con un consumo estimado de 1980 W (≈ 9A), se incorporó una térmica de 16 A, adecuada para el nivel de potencia requerido.
- Protección general del rack: definida en 20 A, lo que equivale a una potencia máxima de ≈ 4400 W, coincidente con la capacidad de transporte del cable conductor de 2,5 mm².
De esta manera, cada protección se seleccionó en función de la potencia real de los equipos y la capacidad de los conductores, evitando tanto sobredimensionamientos que comprometan la seguridad, como sub-dimensionamientos que afecten la continuidad de servicio.
<p align="center"> Datasheet “Catálogo - Cable Unipolar Flexible Argenplass”

En la instalación se seleccionó un interruptor diferencial 25A-30 mA, en conjunto con un interruptor termomagnético general de 20 A. Esta configuración asegura la correcta coordinación entre protecciones, ya que el disyuntor diferencial no tiene función de protección contra sobrecorriente, sino contra fugas a tierra, mientras que la limitación de corriente queda a cargo del interruptor termomagnético. Al disponer un térmico de 20A aguas arriba, se garantiza que el diferencial de 25A no sea sobrecargado, manteniendo la seguridad tanto del cableado como de los equipos conectados, y asegurando la protección de las personas frente a contactos indirectos mediante la sensibilidad de 30 mA.

#### 3.4.6 Plano Unifilar de Rack01 industrial  
<p align="center">
  <img width="2482" height="1755" alt="(TOR) Unifilar de Rack" src="https://github.com/user-attachments/assets/931a9de6-dc55-4890-8f0d-f70f509420d3" />
  <br>
  <em>Figura 9: Plano Unifilar de Rack01 industrial </em>
</p>

### 3.4.7 Documentación estándar 
Finalmente, se generó documentación estándar que servirá como referencia para futuros proyectos de redes industriales dentro de la empresa.

---

## 4. Conclusiones
A partir de la Práctica Profesional Supervisada permitió establecer las bases para el desarrollo de una red industrial en Saint-Gobain, Weber Tortuguitas. El trabajo realizado incluye estudio de normativa, relevamiento de equipos y elaboración de documentación de ingeniería, aportando a la empresa una infraestructura estandarizada y escalable, esencial para construir los cimientos que permitirán a futuro la implementación de un SCADA Centralizado y para avanzar en el proceso de digitalización dentro del marco de Industria 4.0. 

---

## 🤝 Contacto

- **Reynaga Rios Leandro Joel**  
  - 📬Email: leandro_05_01@hotmail.com  
  - GitHub: [@LeandroReynaga](https://github.com/LeandroReynaga)

---




