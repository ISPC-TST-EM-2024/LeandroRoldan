![logo](/.rsc/img/Logo.png)

# TP3 - Circuito Lógico Combinacional - 

###  Docente: *Gustavo Vera*
### Alumno: *Patricio Leandro Roldan* 

---  
  
### Implementación de una función lógica:  

Se diseñó un circuito combinacional que implementa la función lógica F(A, B, C) = A'B + AC.

![01](https://github.com/ISPC-TST-EM-2024/LeandroRoldan/blob/main/TP%203/C%20Prototipos/compuertas%201.png)  

---  



## Simplificación de una expresión lógica:  

Se simplifica con la expresion lógica **"F(A,B, C, D) = ABC + AB'D + ACD"**  con algebra de boole

F(A,B, C, D) = **ABC + AB'D** + ACD'  

{Propiedad distibutiva}  

F(A, B, C, D) = *AB(C+D)* + **ACD**

{Propiedad Distributiva}    
F(A,B,C,D) = AB(C+D) + *AC(D+B)*

{Propiedad Conmutativa }  

F(A,B,C,D) = AB(C+D) + ACD+ACD   

{Idempotencia}  
F(A,B,C,D) = AB(C+D) + AC


  #### La expresion simplificada es **F(A,B,C,D) = AB(C+D) + AC**





  
  Para realizar este mismo procedimiento con mapa de Karnaugh.  
    Sea la tabla   

| A 	| B 	| C 	| D 	| F 	|
|---	|---	|---	|---	|---	|
| 0 	| 0 	| 0 	| 0 	| 0 	|
| 0 	| 0 	| 0 	| 1 	| 0 	|
| 0 	| 0 	| 1 	| 0 	| 1 	|
| 0 	| 0 	| 1 	| 1 	| 0 	|
| 0 	| 1 	| 0 	| 0 	| 0 	|
| 0 	| 1 	| 0 	| 1 	| 1 	|
| 0 	| 1 	| 1 	| 0 	| 1 	|
| 0 	| 1 	| 1 	| 1 	| 0 	|
| 1 	| 0 	| 0 	| 0 	| 0 	|
| 1 	| 0 	| 0 	| 1 	| 1 	|
| 1 	| 0 	| 1 	| 0 	| 1 	|
| 1 	| 0 	| 1 	| 1 	| 0 	|
| 1 	| 1 	| 0 	| 0 	| 1 	|
| 1 	| 1 	| 0 	| 1 	| 1 	|
| 1 	| 1 	| 1 	| 0 	| 1 	|
| 1 	| 1 	| 1 	| 1 	| 0 	|  

Se Genera el mapa K de la siguiente forma:

| AB\CD	| 00 	| 01 	| 11 	| 10 	|
|---	  |---	|---	|---	|---	|
| 00 	| 0 	| 0 	| 0 	| 1 	|
| 01 	| 0 	| 1 	| 0 	| 1 	|
| 11 	| 1 	| 1 	| 0 	| 1 	|
| 10 	| 0 	| 1 	| 0 	| 1 	|    
  
Formando asi 4 grupos
**F = CD' + AC'D + ABD' + BC'D**


A pesar de haber llegado a Expresiones diferentes, las tres son equivalentes.

---  


## Multiplexor:  

Se diseño un circuito combinacional simple para implentar un multiplexor (Mux) 4x1, Utilizando compuertas lógicas:  

![mux](https://github.com/ISPC-TST-EM-2024/LeandroRoldan/blob/main/TP%203/C%20Prototipos/03%20circuito.png)   


Con su tabla de verdad:  

![Tabla_mux](https://github.com/ISPC-TST-EM-2024/LeandroRoldan/blob/main/TP%203/C%20Prototipos/03%20tabla%20de%20verdad.png) 

---  


## Comparador de números de 2 bits:  

Se diseñó un circuito combinacional que compara dos numeros de 2 bits, y produce una salida de 1 si A > B, 0 So A==B, y -1 Si A < B.  
Para ello se realizó el siguiente esquema:  

![04_esquema](https://github.com/ISPC-TST-EM-2024/LeandroRoldan/blob/main/TP%203/C%20Prototipos/04_circuito1.png)  
Por lo que cada salida, S0, S1 y S2, representan el valor 1,0,-1 respectivamente. con la respectiva tabla de verdad:  

![04_tabla](https://github.com/ISPC-TST-EM-2024/LeandroRoldan/blob/main/TP%203/C%20Prototipos/04%20tabla%20de%20verdad.png)   

Y sus Mapas K:  

![04_Mapa](https://github.com/ISPC-TST-EM-2024/LeandroRoldan/blob/main/TP%203/C%20Prototipos/04%20Tabla%20K.png)
   

 ---

## Codificador:  

Se diseñó un circuito combinacional que implementa un codificador 4x2, utilizando compuertas lógicas.  

![05_cod](https://github.com/ISPC-TST-EM-2024/LeandroRoldan/blob/main/TP%203/C%20Prototipos/05%20Codificador%204a2.png)  


Y corresponde a la siguiente tabla de verdad:  

![05_tabla](https://github.com/ISPC-TST-EM-2024/LeandroRoldan/blob/main/TP%203/C%20Prototipos/05%20tabla.png)  



Con el mismo se da por finalizado el trabajo practico Numero 3.  A disposicion. 
---  






