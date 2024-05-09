![logo](/.rsc/img/Logo.png)

# TP2 - Simulación Electrónica - 21/04/2024  

###  Docente: *Gustavo Vera*
### Alumno: *Patricio Leandro Roldan* 


### Durante esta semana pude visualizar algunas de las bases en semiconductores, como el diodo, el transistor y el amplificador operacional.


### Diodos 

Pude verificar como en la siguiente imagen:  

![01|300](/TP%202/C%20Prototipos/01.png)  

Que los diodos tienen una alta, o muy baja resistencia, dependiendo de la polaridad de la tension.


![01b|300](/TP%202/C%20Prototipos/01bç.png)  

---
En este caso utilivé leds para evidenciar la barrera que produce diodo ante la conexion en el catodo la tension positiva. y por el contrario, con polarizacion directa, el led D2, se enciende.  


### Transistores
Utilizado para amplificar o cambiar señales y potencias eléctricas proviene del acrónimo *"transfer resistor"*.

Las propiedades que estudié durante esta semana son dos: amplificador, y como interruptor.  

En el primer caso:  

![02|300](/TP%202/C%20Prototipos/02.png)  
El transistor se encuentra conectado como amplificador de potencia.  Siendo la salida de color amarillo, el canal A, La salida amplificada, y en el colector se observa la señal mas debil:  

![02c|300](/TP%202/C%20Prototipos/02OC.png)  
  

En el caso de su uso como interrutor, Se puede observar que con una pequeña tension en la base, se puede lograr el efecto de interruptor entre el emisor y el colector.  
En este ejemplo, utilicé una bateria de 1.5 V para energizar la base, y lograr controlar una tension de 8 V DC entre el emisor y el colector.    

![03|300](/TP%202/C%20Prototipos/03.png)  

Con una bateria de 12V:  

![04|300](/TP%202/C%20Prototipos/04.png)  

  ---

### Amplificadores Operacionales (op-amp):  

Son llamados así porque pueden amplificar con gran ganancia una señal, y porque originalmente, a finales de la década de 1940, surgieron como solución para ejecutar operaciones matemáticas (desde suma y multiplicaciones hasta derivadas e integrales, por citar algunas).  

En el siguiente ejemplo, Conecté un operacional como sumador inversor:  

![05|300](/TP%202/C%20Prototipos/05AC.png)
![05|300](/TP%202/C%20Prototipos/05C.png)    

Se puede observar como de 3 señales de 3V AC, Se obtiene como resultado, luego de pasar por las resistencias y el operacional, a -14V. 

---
  


Finalmente, conecté el operacional *LMH6672* Dual en modo comparador. La implementación se realizó en dos etapas, observando que la salida depende de la comparación de los dos valores de entrada. Estos valores de entrada actúan como un interruptor, controlando el paso de la señal proveniente del suministro, ya sea positiva o negativa, en función de la comparación realizada.  

![06|300](/TP%202/C%20Prototipos/06.png )
![06b|300](/TP%202/C%20Prototipos/06b.png)  



Por ultimo diseñé este comparador unido a resistencias, que gradualmente cae la tension pasando por las resistencias, y asi el valor de comparacion es cada vez menor. De esta forma con una sola señal, se puede analizar y encender la cantidad de leds correpondiente al valor de entrada.
En lo ejemplos siguientes la tension de a comparar es 5.1V y 2V:  


![06|300](/TP%202/C%20Prototipos/061.png)   



![06|300](/TP%202/C%20Prototipos/061b.png)



Siendo asi que se encienden en el primer caso todos los leds, ya que se compara 5.1 V contra 5, 3.3 , 1.7 , y 0 Volts respectivamente. Y, en el segundo caso, se compara 2 volts, por lo que se encienden solo los primeros 2 leds.

