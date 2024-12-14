# Piedra-Papel-Tijera
## 1.Especificación do contorna de tarefas
Contorno de tarefas | Observable| Axentes | Determinista | Episódico | Estático | Discreto | Coñecido
:---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
 RPS | Parcialmente | MultiAgente | No Determinista | Secuencial | Estático |  Discreto |  Coñecido |
 ### Explicación de las carácteristicas del entorno
 #### **Observable**
 Considero que en la categoria de observable, decimos que el entorno es parcialmente observable, por que el agente no puede saber la opción que sacara el rival.
 #### **Agentes**
 Se trata de un entorno de MultiAgentes, ya que el número minimo de jugadores debe ser 2 en adelante.
 #### **Determinista**
 Decimos que el RPS es No-Determinista por que no está determinada la opción que se usará en cada turno según el turno anterior. Podemos plantear una estrategia y tener cierta idea de que es más o menos probable, pero nunca será seguro al 100%
 #### **Episódico**
 De la misma manera que hemos explicado por que RPS es **No-Determinista** podemos decir que es Secuencial ya que no hay una opción que defina el siguiente movimiento del agente. 
 #### **Estático**
 Se define como un entorno Estático debido a que el estado del mundo no cambia una vez que ha tomado la decisión.
 #### **Discreto**
 Decimos que es Discreto, por que las posibles opciones son limitadas, al igual que las combinaciones de estados.
 #### **Conocido** 
 El juego de RPS todos los agentes conocen sus reglas para poder jugarlo, se trata de un mundo pequeño sin posibilidad de descubrir nuevas reglas a medida que juegas.

 ## 2.Identificación del tipo de agente y estructura
 El tipo de agente utilizado para este proyecto será un **agente reactivo basado en un modelo** (Indicado en el punto 2.4.3 del libro "Artificial Intelligence a Modern Approach). Esto se debe a que en la implementación del código guardaremos dos variables goblales para que el agente tome decisiones, se tratan de la variable **result** y **last_user_action**. Además crearemos una clase *GameComputerResult* de tipo enumerado que guardará el estado de la ultima partida y que resultado obtuvo nuestro agente.
