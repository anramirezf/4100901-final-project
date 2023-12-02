# Seguro de bombas mineras
This repository contains the example for the final project of the course computation structures. Please go to the [C4Model](Doc/C4Model.md) diagrams for more details on the functionality of the system.

## Hardware prerequisites
* The example is a digital lock system featuring an STM32L4 for controling the system, an ESP8266 for interfacing with the internet, a keypad for getting the sequences, and an OLED display for GUI. See more details in the [C4Model](Doc/C4Model.md)
* The following is the pinout of the STM32:
![pinout](Doc/pinout.png)

## Firmware prerequisites
* The ESP8266 runs the esp-link [v2.2.3](https://github.com/jeelabs/esp-link/releases/tag/v2.2.3) firmware. Please follow the [serial flashing guide](https://github.com/jeelabs/esp-link/blob/master/FLASHING.md#initial-serial-flashing).
* The STM32 runs the firmware compiled from this repository using STM32CubeIDE.

## Building and Flashing
* Open the project in STM32CubeIDE.
* Compile using the current project settings.
* Use an ST-LINK to flash the firmware into the STM32.

##Introducción
En entornos mineros, donde la seguridad es primordial, la implementación de un seguro de 3 intentos en la activación de bombas se convierte en un componente esencial para salvaguardar vidas y garantizar la integridad de las operaciones. Este enfoque cuidadoso y estratégico busca evitar activaciones accidentales o indebidas de dispositivos explosivos, reduciendo significativamente los riesgos asociados con dichas operaciones.

1. Prevención de Activaciones Accidentales:
La inclusión de un seguro de 3 intentos implica que cualquier intento de activación de la bomba debe ser validado tres veces antes de ejecutarse. Este nivel de seguridad garantiza que no se produzcan activaciones accidentales debido a malentendidos, errores de entrada o fallos en los sistemas de control. La necesidad de confirmación triple actúa como una barrera crítica, reduciendo la probabilidad de eventos no deseados y minimizando las posibles consecuencias catastróficas.

2. Protección contra Errores Humanos:
La operación de equipos en entornos mineros puede ser compleja y desafiante. La presencia de un seguro de 3 intentos proporciona un margen de error razonable, permitiendo a los operadores corregir cualquier malentendido o error de entrada antes de que se realice una activación definitiva. Esto no solo protege al personal de posibles riesgos, sino que también salvaguarda los costosos equipos y la infraestructura asociada.

3. Cumplimiento Normativo y Buenas Prácticas:
En muchos casos, las regulaciones y normativas de seguridad en la industria minera requieren la implementación de medidas de seguridad robustas. Un seguro de 3 intentos no solo cumple con estos requisitos, sino que también demuestra el compromiso de la operación minera con las mejores prácticas de seguridad. Esto puede contribuir positivamente a la reputación de la empresa y fortalecer su posición en el cumplimiento normativo.

4. Reducción de Riesgos para el Personal:
La seguridad del personal es la máxima prioridad en operaciones mineras. Al incorporar un seguro de 3 intentos, se brinda a los trabajadores la tranquilidad de saber que se han implementado medidas adicionales para prevenir activaciones no deseadas. Esto no solo promueve un entorno laboral más seguro, sino que también fomenta la confianza y la moral del equipo.

5. Respuesta Controlada en Caso de Emergencia:
En situaciones de emergencia, tener un seguro de 3 intentos proporciona una ventana de oportunidad para evaluar y gestionar la situación antes de tomar medidas decisivas. Esto permite una respuesta controlada y planificada en lugar de una reacción impulsiva, lo cual es crucial en entornos donde la seguridad es de suma importancia.

En conclusión, la implementación de un seguro de 3 intentos en la activación de bombas en operaciones mineras no solo es una práctica sensata desde el punto de vista de la seguridad, sino que también se alinea con las expectativas regulatorias y las mejores prácticas de la industria. Este enfoque proactivo refleja el compromiso de la empresa con la seguridad y el bienestar de su personal, así como con la sostenibilidad a largo plazo de las operaciones mineras.

## Functionality

The Keypad:
This input device, commonly known as a numeric keypad, plays a critical role in the digital lock system by providing an intuitive interface for users. It allows the input of specific sequences of numbers or characters, acting as the key that authenticates and unlocks the lock. User interaction with this component becomes fundamental, as its precision and effectiveness are crucial for ensuring the security of the system.

The Debug Console:
The debug console not only provides a superficial view but also offers a detailed immersion into the internal functioning of the system. This advanced interface becomes an essential tool for developers and technicians, presenting debug messages, comprehensive logs, and the detection of potential errors. It facilitates the efficient identification and resolution of issues, enabling faster development and continuous improvement of the system.

The Internet Interface:
The capability of the digital lock system to connect through a web interface with the Internet significantly enhances its functionality. This interface enables bidirectional data transmission over the network, allowing precise time synchronization, remote firmware updates, and the reception of important notifications. The web interface becomes the vital link between the system and the vast online world.

The System Sends Data to the Cloud:
The configuration allowing the system to send data to the cloud at regular intervals, every 24 hours in this case, reveals a proactive strategy for remote management and efficient monitoring. This process is achieved through an alarm generated by the integrated Real-Time Clock (RTC) in the system. The data sent to the cloud may include detailed information about the operational status of the system, event logs, usage patterns, and other valuable insights. This not only facilitates continuous tracking but also supports informed decision-making for system maintenance and continuous improvement. In this context, the cloud becomes a centralized repository for the intelligence of the system, facilitating effective remote management.

## Contact info
* Sam C - saacifuentesmu@unal.edu.co
