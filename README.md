# Propósito:

Proyecto de Jordi Garcia Castillón - ONCE (Hackathon for Good - La Región de AWS en España al servicio de la sociedad): Visión por computador para personas con discapaciad visual.

# Solución propuesta e impacto social:

Este sistema simplemente está pensado para ser un aplicativo base para “proveer” a cualquier otro sistema o elemento (dicho de otro modo, se trata de proveer de una API que puede ser integrada y consumida desde cualquier dispositivo de la persona con discapacidad visual total o parcial) de la funcionalidad para el que ha sido preparado, y todo ello por lo siguiente:

Este sistema está centrado en proveer de las siguientes funcionalidades elementales:

Mediante el reconocimiento de imágenes se pretende que la persona con discapacidad pueda circular de una forma más autónoma y segura por el "supermercado" (o cualquier otra gran superficie).

La configuración de este sistema podría darse de distintas maneras, pero en este caso se ha planteado específicamente para que la persona usuaria del sistema pueda detectar al personal trabajador del supermercado en cuestión o pueda detectar los puntos de atención al cliente que estén señalizados con simbología reconocible con la imagen corporativa del establecimiento.

La finalidad de todo ello es que la persona pueda disponer de más independencia y comodidad en su compra y, especialmente, que cuando requiera de hacer alguna pregunta o realizar cualquier gestión con el personal del supermercado o centro comercial pueda detectar a dichas personas o puntos de atención automáticamente sin tener que preguntar a terceros por su localización.

# Introducción técnica y disclaimer:

Este proyecto se ha desarrollado únicamente con fines de demostración prototipo para el Hackathon for Good (https://www.hackathoniberia.com/), organizado por AWS entre el 26 de abril y el 10 de mayo del 2023.

La fuente de datos primeria (el dataset) se ha generado artificialmente mediante IA generativa. Creando imágenes de personas (y carteles) vestidas con la indumentaria de un imaginado centro comercial.

El estado actual de desarrollo no habilita al mismo en estos momentos para sus usos en producción de ningún tipo.

Tanto los resultados obtenidos como la funcionalidad misma de este desarrollo tan sólo puede interpretarse por ahora como una mera demostración básica, pues se encuentra en un estado funcional pero evidentemente ni la cantidad de imágenes con las que se ha preparado el sistema ni muchas otras variables o consideraciones hacen que la fiabilidad en producción de este desarrollo esté ahora ni mucho menos establecida.

# Implementación técnica resumida:

Bucket en S3 para el dataset en la región de España (https://aws.amazon.com/es/local/spain/)

Entrenamiento e inferencia con AMAZON REKOGNITION (https://aws.amazon.com/es/rekognition/)

(en el dataset para un balanceo adecuado se pretende dotar una equivalencia entre imágenes que representen ciertamente la imagen corporativa del supermercado / centro comercial, imágenes que sean antagonistas de dicha imagen corporativa e imágenes que puedan resultar dudosas. Por ello será necesaria una continua retroalimentación del modelo hasta conseguir una robustez elevada)

# Notas finales: 

Los miembros del jurado pueden solicitarme el acceso al recurso en Rekognition, a la API en el momento que lo deseen para poder comprobar el funcionamiento del sistema si lo desean.

Link al video del proyecto: 
