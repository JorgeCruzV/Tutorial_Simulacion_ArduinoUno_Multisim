# Tutorial_Simulacion_ArduinoUno_Multisim
 
TUTORIAL PARA SIMULAR PROGRAMAS EN UN EQUIVALENTE DE ARDUINO UNO EN MULTISIM

1)	MARCO TEÓRICO 


a)	Arduino 

Arduino es una plataforma de creación de electrónica de código abierto, la cual está basada en hardware y software libre, flexible y fácil de utilizar para los creadores y desarrolladores. Esta plataforma permite crear diferentes tipos de microordenadores de una sola placa a los que la comunidad de creadores puede darles diferentes tipos de uso.

Para poder entender este concepto, primero vas a tener que entender los conceptos de hardware libre y el software libre. El hardware libre son los dispositivos cuyas especificaciones y diagramas son de acceso público, de manera que cualquiera puede replicarlos. Esto quiere decir que Arduino ofrece las bases para que cualquier otra persona o empresa pueda crear sus propias placas, pudiendo ser diferentes entre ellas, pero igualmente funcionales al partir de la misma base.

El software libre son los programas informáticos cuyo código es accesible por cualquiera para que quien quiera pueda utilizarlo y modificarlo. Arduino ofrece la plataforma Arduino IDE (Entorno de Desarrollo Integrado), que es un entorno de programación con el que cualquiera puede crear aplicaciones para las placas Arduino, de manera que se les puede dar todo tipo de utilidades.

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/1.jpg)


 

i)	Arduino Uno 

La placa Arduino UNO es la mejor placa para iniciar con la programación y la electrónica. Si es tu primera experiencia con la plataforma Arduino, la Arduino UNO es la opción más robusta, más usada y con mayor cantidad de documentación de toda la familia Arduino.

Arduino UNO es una placa basada en el microcontrolador ATmega328P. Tiene 14 pines de entrada/salida digital (de los cuales 6 pueden ser usando con PWM), 6 entradas analógicas, un cristal de 16Mhz, conexión USB, conector Jack de alimentación, terminales para conexión ICSP y un botón de reseteo. Tiene toda la electrónica necesaria para que el microcontrolador opere, simplemente hay que conectarlo a la energía por el puerto USB o con un transformador AC-DC

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/2.png)

 
	ii)	Características del Arduino uno.

• Corriente DC por pin de E/S: 40 mA

• Corriente DC para 3.3V Pin: 50 mA

• Memoria Flash: 32 KB de los cuales 0,5 KB utilizados por el bootloader

• SRAM: 2 KB (ATmega328)

• EEPROM: 1 KB (ATmega328)

• Microcontrolador: ATmega328

• Voltaje de operación: 5V

• Voltaje de entrada (recomendado): 7-12V

• Voltaje de entrada (límites): 6-20V

• Pines de E/S digitales: 14 (de los cuales 6 proporcionan salida PWM)

• Pines de entrada analógica: 6

• Velocidad de reloj: 16 MHz


	iii)	Esquema, componentes y especificaciones de la placa Arduino Uno.

 
![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/3.jpg)


(1)	Botón de reset. Sirve para inicializar nuevamente el programa cargado en el microcontrolador de la placa. Cuando deje de responder el Arduino Uno es el botón de encendido o apagado para que vuelva a restablecerse. 

(2)	2 y 3- Pines o puertos de entrada y salida, son los pines donde conectar los sensores, componentes y actuadores que necesiten de señales digitales.

(3)	Puerto USB. Utilizado tanto para conectar con un ordenador y transferir o cargar los programas al microcontrolador como para dar electricidad al Arduino. También se usa como puerto de transferencia serie a la placa, tanto para transmisión como para recepción de datos.

(4)	Chip de interface USB, es el encargado de controlar la comunicación con el puerto USB.

(5)	Reloj oscilador. Es el elemento que hace que el Arduino vaya ejecutando las instrucciones. Es el encargado de marcar el ritmo al cual se debe ejecutar cada instrucción del programa. 

(6)	Led de encendido. Es un pequeño LED que se ilumina cuando la placa esta correctamente alimentada. 

(7)	Microcontrolador. Este es el cerebro de cualquier placa Arduino. Es el procesador que se encarga de ejecutar las instrucciones de los programas. 

(8)	Regulador de tensión. Este sirve para controlar la cantidad de electricidad que se envía a los pines, con lo que asegura que no se estropee lo que conectemos a dichos pines. 

(9)	Puerto de corriente continua. Este puerto es el que se usa para darle electricidad a la placa si no se usa alimentación USB. 

(10)	Zócalo de tensión. Aquí estarán los pines con los que alimentaremos nuestro circuito. 

(11)	Entradas analógicas. Zócalo con distintos pines de entrada analógica que permiten leer entradas analógicas.


a)	Multisim 14.0

Multisim es un software estándar en la industria para diseño de circuitos y simulación SPICE para electrónica de potencia, analógica y digital en la educación y la investigación.

Multisim integra simulación SPICE estándar en la industria con un entorno esquemático interactivo para visualizar y analizar al instante el comportamiento de los circuitos electrónicos. Multisim tiene una interfaz intuitiva que ayuda a los profesores a reforzar la teoría de circuitos y a mejorar la teoría en todo el plan de estudios de ingeniería. Investigadores y diseñadores utilizan Multisim para reducir las iteraciones de prototipos PCB y ahorrar costos de desarrollo, añadiendo simulación potente de circuitos y análisis al flujo de diseño.


![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/4.jpg)

 

2)	MANUAL DE USUARIO 


a)	Como primer requisito será el tener instalado el Multisim en nuestro ordenador, aquí se puede optar por varios tipos de licencias. 

b)	Como siguiente paso, será el dirigirnos hacia la página oficial de Nacional Instruments, esto para que nuestra descarga sea de una fuente confiable. 

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/5.png)


  

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/6.png)



Aquí podremos observar los requisitos, en el cual se menciona que debemos contar con versión 13.0 y posteriores para poder usar estas herramientas. 

c)	Aquí encontraremos el link de la descarga

 

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/7.png)


d)	Crearemos una carpeta llamada Arduino Library en la carpeta que se nos genera en Mis Documentos Llamada National Insrument 

En mi caso se usó la siguiente dirección:

E:\Datos\OneDrive\Documents\National Instruments\Circuit Design Suite 14.1\Arduino Library


![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/8.png)
![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/9.png)
![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/10.png)

   
 
e)	En esta carpeta copiaremos lo descargado previamente. 


![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/11.png)

 

f)	Aquí extraeremos el archivo tipo zip, donde nos aparecerá una variedad de archivos. Y ya tendríamos las librerías en nuestro ordenador 

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/12.png)

 
1)	EJECUCIÓN DEL PROYECTO  

a)	Abriremos el Multisim

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/13.png)

 
b)	Accederemos en la barra de herramientas a la opción Archivo y luego abrir. 

2)	![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/14.png)


a)	Debemos dirigirnos a la ubicación donde se guardaron y se descomprimieron los archivos.

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/15.png)

 

b)	Aquí escogemos la opción de Arduino uno 


![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/16.png)

![]( https://github.com/JorgeCruzV/Tutorial_Simulacion_ArduinoUno_Multisim/blob/master/Imagenes/17.png)


   
