# Mini - Proyecto #3 I2C y NeoPixel
Objetivo
Con este proyecto se busca que el estudiante experimente con los
microcontroladores STM32F446RE y ESP32 para realizar una aplicación utilizando el
protocolo de comunicación I2C, una pantalla TFT ILI9341 y un led RGB NeoPixel.
Instrucciones Generales
El proyecto consiste en implementar un data logger con un sensor utilizando el
almacenamiento SD además de tener una interfaz gráfica para desplegar los resultados
de las mediciones en la pantalla. El sensor estará conectado al microcontrolador ESP32
el cual tendrá que comunicarse con este utilizando el protocolo de comunicación I2C y
tendrá que enviar la información tanto al microcontrolador STM32F446RE como a la
computadora mediante comunicación UART. Adicionalmente se tendrán dos botones en
el microcontrolador STM32F446RE para seleccionar la tarea que se desea realizar.
También se tendrá un indicador visual utilizando un led RGB NeoPixel.
NOTA: Deberá implementar librerías en sus códigos.
# Parte 1 ESP32:
Diseñe e implemente una rutina en la que el microcontrolador ESP32 se
comunique con un sensor de su elección utilizando el protocolo I2C.
El programa debe realizar la lectura de los datos del sensor y transmitirlos
cuando otro dispositivo los solicite.
# Parte 2 Comunicación UART:
Diseñe e implemente una rutina en el microcontrolador STM32F446RE que
permita solicitar el valor del sensor al ESP32 presionando uno de los botones
del sistema. Cuando el ESP32 reciba la solicitud, deberá enviar el dato del
sensor al STM32 a través de UART. Posteriormente, el STM32F446RE deberá
reenviar dicho dato a la computadora mediante un segundo canal UART.
Nota: Tome en cuenta que debe utilizar 2 canales distintos de UART, uno para
comunicarse con el ESP32 y otro para comunicarse con la computadora.
# Parte 3 Despliegue de datos:
Diseñe e implemente una rutina que permita visualizar en una pantalla TFT el
valor obtenido del sensor. Sea creativo en el diseño de la interfaz gráfica: no se
acepta únicamente texto plano. El despliegue debe ser claro, informativo y
visualmente atractivo.
# Parte 4 Almacenamiento de la SD:
Implemente la comunicación con una tarjeta SD para registrar el valor del
sensor. La escritura del dato en la memoria deberá activarse mediante el
segundo botón disponible en el sistema.
# Parte 5 Indicador Visual:
Implemente un indicador visual utilizando un LED RGB NeoPixel que muestre
los diferentes estados de operación del sistema (por ejemplo: encendido,
midiendo, transmitiendo, guardando datos, etc.). Defina una convención de
colores coherente para representar cada estado.
