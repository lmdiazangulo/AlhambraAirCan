# Alhambra Air Can

## Resumen
*Alhambra Air Can es un proyecto que se propone crear un respirador activo de purificación de aire (powered air purifying respirator, PAPR) de dos vías (entrada y salida).*

## Descarga de responsabilidades
Este documento no constituye un documento que cumpla estándares científicos, es sencillamente una explicación de las desventajas principales de los sistemas de mascarilla convencional, las características principales de un sistema PAPR (Powered Air Purifying Respirator) y una serie de mejoras que pretendemos introducir. 

## Introducción 

Probablemente las mascarillas, en sus diferentes variantes (quirúrgica, FPPx, …) constituyen el principal equipo de protección individual (EPI) de uso masivo por parte de la población. A pesar de su uso tan extendido, presentan distintos problemas para un uso continuado:

1. En un uso continuado, se acumula aire caliente y húmedo que genera una sensación grande de incomodidad. También se ha atribuido como un factor contribuyente a la aparición de agentes infecciosos en el entorno de la boca (hongos, etc). A medida que las condiciones ambientales se vuelven cada vez más extremas, por la llegada del calor, estos problemas se agravan considerablemente.
2. En los procesos de inspiración-espiración, la proporción de gases en la vía respiratoria no tiene una proporción óptima de concentración de gases, pasando a acumularse una mayor proporción de CO2. 
3. Exige un esfuerzo adicional por parte del usuario al requerir una sobrepresión para que el flujo de aire atraviese el filtro de la mascarilla. Este sobreesfuerzo genera cansancio en el usuario.
4. No protegen los ojos, partes húmedas que quedan expuestas a agentes patógenos y alérgenos.
5. Para los usuarios que necesitan gafas resultan problemáticas al empañarse durante la espiración; dificultando la visión. Esto es especialmente problemático en tareas en las que la visión resulta esencial para la seguridad, como por ejemplo conducir.
6. No está comprobada la influencia del vello facial en la eficiencia de filtrado. Probablemente se vería muy reducida al haber huecos recubiertos de vello que no quedan cubiertos por la mascarilla [1].
7. Las mascarillas normalmente están optimizadas para optimizar la protección personal (FPPx) o para evitar contagios (quirúrgicas); pero no ambas simultáneamente.

Algunos de estos factores suponen una falta de confort que, en la práctica, supone un serio riesgo para la seguridad. No es difícil ver en la calle a personas o trabajadores que tienen la mascarilla bajada; o a personas que no pueden evitar tocarse constantemente las manos con las mascarillas. En estas condiciones, su efectividad resulta más que cuestionable ya que precisamente se está tocando el sitio donde más se acumularían los agentes patógenos. Cabe mencionar que la supuesta efectividad del 99% de una mascarilla FPP3 se calcula exclusivamente mediante la capacidad de filtrado del tejido, no teniendo en cuenta las aberturas que presenta, la forma específica de la misma, o su capacidad de adaptarse a la morfología del usuario.


## Sistemas PAPR
Entre las alternativas a las mascarillas respiratorias, en este documento nos centraremos en los sistemas PAPR (Powered Air Purifying Respirator). Los PAPRs son EPIs cuyo funcionamiento consiste en generar una zona presión manométrica positiva en las vías respiratorias del usuario. Esta presión se consigue mediante un sistema de ventilación que eleva la presión dentro de la máscara mediante el influjo de aire ambiente filtrado. La efectividad de protección real  de los equipos PAPR es muy superior al de las mascarillas N95 y FPP (Figura 1) al incluirse más factores que únicamente la capacidad de filtrado del tejido.

![Comparativa de la efectividad real de sistemas PAPR y sistemas N95 (similar a FPP2)](https://open-mask.org/wp-content/uploads/2020/04/PAPRvN95Chart1-768x435.jpg)
    Figura 1: Comparativa de la efectividad real de sistemas PAPR y sistemas N95 (similar a FPP2) (https://open-mask.org)


Algunas compañías ofrecen sistemas PAPR como producto comercial (3M[1]) y también hay varios desarrollos abiertos (Coronavirus Makers[2], open-mask[3]). A continuación describimos brevemente el desarrollo de open-mask, siendo el resto de los estudiados muy similares. Este sistema se puede dividir en dos sub-sistemas (Figura 2):
1. Soplador (blower)[4]. Es la caja que contiene un filtro HEPA[5], con una turbina que fuerza el paso de aire a través de él. El sistema tiene un potenciómetro que permite regular la velocidad de paso de aire. El flujo con el aire ya filtrado es canalizado a través de una tubuladura a la capucha. Consta de una batería alimentada a 12V.
2. Capucha (headgear)[6]. La capucha está hecha de un tejido similar al de las mascarillas quirúrgicas, con la idea de que sean desechables parcialmente. La capucha recubre totalmente la cabeza y se ajusta mediante unas gomas elásticas por en la nuca y base de la mandíbula, formando un receptáculo cerrado. El flujo de aire del soplador, genera una presión positiva dentro del receptáculo, que se va filtrando al exterior a través del tejido.


  
![Sistema PAPR formado por capucha y soplador (wikipedia)](https://upload.wikimedia.org/wikipedia/commons/8/86/Influenza_virus_research.jpg)
Figura 2: Sistema PAPR formado por capucha y soplador (wikipedia).


Este sistema soluciona todos los problemas descritos en la sección anterior presentados por las mascarillas convencionales. Otras ventajas que podríamos destacar de este sistema son las siguientes (traducidas de open-mask.org): 
1. Mejora del confort de usuario y reducción de fatiga debido a un uso continuado.
2. No es necesario un ajuste complejo de la máscara mediante formación y reglamentación.
3. Permite un uso sobre distintos tipos de vello facial y estilos de corte de pelo.
4. Recargable, reusable, y redistribuible a lo largo de muchos ciclos de servicio.
5. Al haber un flujo de aire constante, se garantiza que el aire está a temperatura y humedad relativa y en la proporción de gases del ambiente


A pesar de sus ventajas, los sistemas PAPR son empleados casi exclusivamente en contextos especializados (UCIs, salas de contención, como parte de trajes NBQ, etc). Esta falta de adopción masiva se debe posiblemente a su alto precio (3M, entorno a 1000€, disponible a través de RS Online[7]) o a la falta de capacidad para realizar una producción que cumpla estándares de fabricación y/o el cumplimiento de las normativas aplicables (Coronavirus Makers, open-mask).


## Mejora propuesta
En esta sección, se proponen algunas mejoras del sistema PAPR que se ha descrito. Los problemas que se intentan solucionar son los siguientes:

1. En el sistema descrito, la liberación de la presión positiva en la capucha se realiza a través del tejido de la misma. Esta liberación es bastante irregular, dependiendo de la colocación de la capucha sobre la cabeza. Esto hace que haya una variabilidad considerable en la presión positiva interna.
2. Si bien la presión positiva facilita la inspiración, también dificulta parcialmente la espiración.
3. La filtración por parte de los tejidos de la capucha es debida al tejido, siendo típicamente del 95% para los empleados en mascarillas quirúrgicas. De este modo, si bien se trata de un buen equipo de protección, no garantiza que el usuario no pueda transmitir patógenos a terceras personas.
4. El paso de un flujo de aire permanentemente genera sequedad en los ojos después de un uso continuado.

Para atajar estos problemas, se proponen las siguientes modificaciones:
1. Sustituir la capucha por una máscara (tipo máscara de buceo[8] o similar) modificada mediante un adaptador para aceptar tubuladura estándar de 22 mm de diámetro. El empleo de estos componentes estandarizados abarata los costes, y permite que sean totalmente reutilizables.
2. El exceso de presión dentro de la máscara se libera mediante un segundo tubo, de un 10 mm de diámetro que retorna al soplador. Dentro del soplador es pasado por un segundo filtro HEPA antes de ser liberado al exterior.
3. Estos cambios permiten ampliar la variedad de máscaras a utilizar, al no estar únicamente limitados a una capucha filtradora. Se podría estudiar el uso de mascarillas que cubran la mitad de la cara para evitar la sequedad de los ojos al pasar un flujo de aire constante.

Otras modificaciones que, no siendo fundamentales, pueden mejorar el desempeño y la comodidad del sistema son:
4. Añadir una segunda turbina en la salida para asegurar un flujo constante de aire dentro del sistema.
5. Añadir un sistema de refrigeración de aire que podría hacer más agradable llevar máscara que no llevarla en ambientes muy calurosos.
6. Añadir un detector diferencial de presión que regule la turbina.
7. Sincronizar la activación de la turbinas con las respiraciones por minuto del usuario. De esta forma se reduciría tanto el consumo energético del dispositivo, como la sequedad de los ojos y la presión espiratoria al ciclarse el aire solo durante la inspiración.

## Trabajo futuro
1. Replicar modelo de open-mask.org
2. Introducir las mejoras descritas en el modelo de open-mask.




# Referencias




  

Diferentes versiones del Alhambra Air Can (izquierda y centro), junto con el soplador de Open-Mask (derecha)


  

Ensayo preliminar con una mascara de Decathlon (que no corresponde a la versión final) realizada en el centro IAVANTE, en que se comprobó que los parámetros de flujo era compatibles con la respiración humana.
________________

[1]: "3M™ Versaflo™ TR-300, TR-300+, TR-600 and TR-800 ...." https://multimedia.3m.com/mws/media/1290291O/versaflo-tr-300-vs-tr-600-chart.pdf. Se consultó el 27 may.. 2020.

[2]: "CoronavirusMakers · GitLab." https://gitlab.com/coronavirusmakers. Se consultó el 27 may.. 2020.

[3]: "Open-Mask – Open Powered Air Purifying Respirator." https://open-mask.org/. Se consultó el 27 may.. 2020.

[4]: "Blower Instructions – Open-Mask." 27 abr.. 2020, https://open-mask.org/instructions/blower-instructions/. Se consultó el 27 may.. 2020.

[5]: High Efficiency Particulate Air

[6]: "Headgear Instructions – Open-Mask." https://open-mask.org/instructions/head-gear-instructions/. Se consultó el 27 may.. 2020.

[7]: "RS Components | Su partner digital de soluciones industriales." https://es.rs-online.com/web/. Se consultó el 27 may.. 2020.

[8] "Máscara de snorkel en superficie Easybreath azul ... - Decathlon." https://www.decathlon.es/es/p/mascara-de-snorkel-en-superficie-easybreath-azul/_/R-p-1616. Se consultó el 27 may.. 2020.
