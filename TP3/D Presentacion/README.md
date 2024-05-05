![logo](/.rsc/img/Logo.png)

# TP3 - Circuito Lógico Combinacional - 

###  Docente: *Gustavo Vera*
### Alumno: *Patricio Leandro Roldan* 


### 1 Implementación de una función lógica:  

Se diseñó un circuito combinacional que implementa la función lógica F(A, B, C) = A'B + AC.

![01](/C%20Prototipos/compuertas%201.png)  

---  



## Simplificación de una expresión lógica:  

Se simplifica con la expresion lógica **"F(A,B, C, D) = ABC + AB'D + ACD"**  con algebra de boole

F(A,B, C, D) = ABC + AB'D + ACD'  
{Propiedad distibutiva}  

F(A, B, C, D) = ABC + AB'D + ACD' = AB(C + D') + AC(D')  
{Se factoriza TC}  

F(A, B, C, D) = AB(C + D') + AC(D') = B(AC + D') + AC(D')  
{Propiedad asociativa}  

F(A, B, C, D) = B(AC + D') + AC(D') = AC(B + D') + B(D')  

{prop conmutativa}  
F(A, B, C, D) = AC(B + D') + B(D') = AC(D' + B) + B(D')  

{Se agrupa en terminos}  
F(A, B, C, D) = B(D' + AC) + AC(D')  

{Ley de absorcion}  
F(A, B, C, D) = B(AC + D') = B(AC) + B(D') = ABD + BD'  
  
  
Exprecion terminada:  F(A, B, C, D) = ABD + BD'    

  
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

| Mapa CD/AB	| 00 	| 01 	| 11 	| 10 	|
|---	  |---	|---	|---	|---	|
| 00 	| 0 	| 0 	| 0 	| 1 	|
| 01 	| 0 	| 1 	| 0 	| 1 	|
| 11 	| 1 	| 1 	| 0 	| 1 	|
| 10 	| 0 	| 1 	| 0 	| 1 	|  


