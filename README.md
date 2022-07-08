# CIRCUITOS-LAB-5

![image](https://user-images.githubusercontent.com/105686218/169063263-fec46540-3f80-4755-af10-c6e466470348.png)        

## CARRERA DE ELECTRONICA Y AUTOMATIZACION

## FUNDAMENTOS DE CIRCUITOS ELECTRICOS

***

**1. Objetivos**

***

   **1.1. Objetivo General** 

Comprobar el Teorema de Thévenin, mediante el análisis del circuito eléctrico, simulaciones y las prácticas de laboratorio experimentales, para afianzar los conocimientos adquiridos sobre el tema propuesto.
***

  **1.2. Objetivos Específicos:**
- Construir mapas conceptuales que resuman el Teorema de Thévenin, a partir de una búsqueda bibliográfica.

- Calcular el valor de voltaje y corriente que pasa por una resistencia, mediante la medición experimental del circuito, medición en el simulador de Tinkercad y analíticamente utilizando Thévenin.

- Justificar el desarrollo del laboratorio, mediante la presentación de un video, que explique la resolución del Teorema de Thévenin, la construcción y funcionamiento del circuito.

- Comparar los resultados que se obtienen analíticamente, simuladamente y experimentalmente.
***

**2. Marco Teórico**

![image](https://user-images.githubusercontent.com/105686218/177908897-e1af3d07-b916-4b40-8276-b1a226fdfa78.png)

![image](https://user-images.githubusercontent.com/105686218/177908921-65a9ecb0-deba-48d4-a5f5-3daaa297b6ee.png)

![image](https://user-images.githubusercontent.com/105686218/177908945-cfa209b4-4729-453b-a927-d51dd06854e8.png)

![image](https://user-images.githubusercontent.com/105686218/177909010-df0eb4ad-789a-4643-91ff-aa0638b379ce.png)

![image](https://user-images.githubusercontent.com/105686218/177909297-0b6877b4-9b65-4b99-b15f-ff0dd320a92f.png)

![image](https://user-images.githubusercontent.com/105686218/177909317-02ca0ae4-b064-44ab-9524-80b20289356e.png)

![image](https://user-images.githubusercontent.com/105686218/177909343-a806d81d-f651-4f77-9568-69e9f8557c07.png)

![image](https://user-images.githubusercontent.com/105686218/177909375-9d80c0a9-c55c-43dc-8bc5-797c2a7757d4.png)



***

**3. Procedimiento**

![image](https://user-images.githubusercontent.com/94011974/177994855-e069a065-df4f-4d5e-85e9-1c86822b71ac.png)

Calculamos el voltaje y la corriente del resistor 5 usando analisis de mallas.

Ecuacion 1 

-10 + 0.56(I1) + 4.7(I1-I2) = 0

Ecuacion 2

-2 + 0.33(I2-I3) + 4.7 (I2-I1) = 0

Ecuacion 3

0.10(I3) + (I3) + 0.33(I3-I2) = 0

Resolviendo en un solucionador de ecuaciones

![image](https://user-images.githubusercontent.com/94011974/177995827-2eb537e4-bd88-4d8f-aac9-bd2a81bf59f1.png)

I1 = 14.86 mA
 
I2 = 14.5 mA

I3 = 3.34 mA

Calculamos voltaje de R5 con ley de ohm

V = I/R = 3.34/1 = 3.34V

Voltaje y corriente de R5 es

I3 = 3.34

VR5 = 3.34

Para encontrar el volatje de Thévenin lo primero que se va a hacer es eliminar R5

![image](https://user-images.githubusercontent.com/94011974/177999073-9e750f45-2176-4e83-9e80-8c134ea68b4b.png)

Se va a usar las ecuciones del analiss de mallas, tomando en cuando que solo va a existir dos mallas ya que en R5 caen 0V porque no hay corriente, entonces esta resistencia no va a afectar los calculos

Ecuacion 1 

-10 + 0.56(I1) + 4.7(I1-I2) = 0

Ecuacion 2

-2 + 0.33(I2) + 4.7 (I2-I1) = 0

Usando solucionador de ecuaciones hallamos que:

![image](https://user-images.githubusercontent.com/94011974/177999333-0256e752-4582-4df1-87e5-9ce978dc5e68.png)

I1 = 13.67 mA

I2 = 13.17 mA

Vthevenin = (13.17)(0.33) = 4.35 V

Para encontrar la resistencia de Thévenin, lo primero que se va a hacer es reemplazar las fuentes de voltajes por sus resistencias internas para posteriormente encontrar las resistencia total.

![image](https://user-images.githubusercontent.com/94011974/177989223-bf84b7ee-2d82-47b8-9902-3dc44fb376dd.png)

Re = ((0.56)(4.7))/0.56+4.7 = 0.500

Re = ((0.500)(0.33))/0.500+0.33 = 0.199 + 0.10 = 0.299 kohm = 299 ohm

Entonces se tiene el voltaje y resistencia de thevenin

VTH = 4.35 V

RTH = 299 ohms

El circuito equivalente.

![image](https://user-images.githubusercontent.com/94011974/178000023-ca3b05e1-93a2-43ab-9e6c-6dff328a5e80.png)

encontramos voltaje y corrinete en R5

VR5 = (1/(1+0.299))(4.35) = 3.35 V

IR5 = 3.35/1 = 3.35 mA

**5. Respuestas a interrogantes**

5.5.1. Arme el circuito que se muestra en la figura 5.1.

![image](https://user-images.githubusercontent.com/94011974/178000800-92cca250-3db6-4705-987d-2f0af87d7dc5.png)

5.5.2. Mida el voltaje y la corriente en el resistor R5, anote los resultados en la tabla 5.2.

![image](https://user-images.githubusercontent.com/94011974/178000695-7a9c3a06-a9c5-40ec-9b6a-e31be65f9064.png)

5.5.3. Desconecte el resistor R5 y mida el voltaje en el circuito abierto. Anote el valor medido en la tabla 5.1.

![image](https://user-images.githubusercontent.com/94011974/178001015-455b615d-8553-45d5-b0c5-7130b219bb26.png)

5.5.4. Anule el efecto de las fuentes de alimentación. Desconecte R5 y desde el circuito abierto resultante mida la resistencia equivalente. Anote el valor medido en la tabla 5.1.

![image](https://user-images.githubusercontent.com/94011974/178001145-84396beb-56ef-43d9-8443-3ad41cdf2533.png)

5.5.5. Implemente el circuito equivalente de Thévenin, agregue el resistor R5 y mida la corriente y el voltaje en el mismo, anote los resultados en la tabla 5.2.

![image](https://user-images.githubusercontent.com/94011974/178002022-7874e569-2453-4585-a38c-c243b558ac76.png)

Tabla 5.1. Valores del Circuito Equivalente de Thévenin

![image](https://user-images.githubusercontent.com/94011974/178003331-de90f9fa-7206-45db-be0f-62b30af00b9f.png)

Tabla 5.2. Comprobación del Teorema de Thévenin.

![image](https://user-images.githubusercontent.com/94011974/178003368-f4132984-a9ed-4e66-9e79-6980a3141527.png)

***

**6. Cálculo de error**

![image](https://user-images.githubusercontent.com/94011974/170057592-12d7c136-22cd-4cac-9532-0e92eb81f1b9.png)

***

**7. Vídeo**

***

**8. Conclusiones**
- A partir de lo investigado anteriormente, se puede concluir que el Teorema de Thévenin, se utiliza cuando queremos simplificar un circuito, expresándolo con una fuente de voltaje equivalente y una resistencia equivalente. Los valores que se obtienen dependen del circuito original. Para encontrar la resistencia equivalente no se deben poner la resistencia de carga, esta se la reemplaza por un circuito abierto y las fuentes de voltaje se las reemplaza por sus resistencias internas, mientras que en el voltaje equivalente se halla el voltaje del circuito abierto presente entre dos terminales de salida.

- Como se ha podido observar se realizó el cálculo de las medidas de voltaje y corriente en R5, se construyó el circuito indicado y con la ayuda de un multímetro se tomó las medidas experimentales cuando se desconecta R5, se anula el efecto de las fuentes de alimentacion y el circuito implementado ya el voltaje y corriente equivalente. Después en Tinkercad se hizo una simulación del circuito obteniendo las medidas de voltajes y corrientes simuladas, finalmente se calculó el voltaje y la corriente utilizando el Teorema de Thévenin.

- En la justificación del video se pude observar la construcción del circuito y su funcionamiento, se puede ver como se toman las medidas indicadas, también la construcción del circuito en el simulador de Tinkercad y su toma de medidas mediante simulación, se explica el análisis que se realizó para el Teorema de Thévenin.

- Analizando el porcentaje de error, se concluye que el voltaje y corriente está correctamente calculado y la variación mínima del error entre los datos calculados y los simulados es por los decimales que se toman en cuenta en los cálculos realizados, mientras que el porcentaje de error entre los valores calculados y experimentales es mayor porque se conoce que los circuitos experimentales se ven afectados por distintos factores.


***

**9. Bibliografía**

Floyd, T. (2007). Principios de circuitos eléctricos. PEARSON Educación. https://drive.google.com/file/d/15UCq2JrPEKKB8SwajlmtTcE07nMiowaK/view

García, A. (29 de marzo de 2021). Ley de corriente de Kirchhoff: Análisis de nodos. Panamahitek. Recuperado de http://panamahitek.com/ley-de-las-corrientes-de-kirchhoff-metodo-de-nodos/

***

10. Rubrica

![image](https://user-images.githubusercontent.com/94011974/169427061-265123c2-f557-4b9a-9ef6-5a545e89aff2.png)
