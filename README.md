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

![image](https://user-images.githubusercontent.com/94011974/177988042-01560dab-33d0-4c9a-930a-87ade73dd921.png)

Calculamos el voltaje y la corriente del resistor 5 usando analisis de mallas.

Ecuacion 1 

-12 + 0.56(I1) + 4.7(I1-I2) = 0

Ecuacion 2

-2 + 0.33(I2-I3) + 4.7 (I2-I1) = 0

Ecuacion 3

0.10(I3) + (I3) + 0.33(I3-I2) = 0

Resolviendo en un solucionador de ecuaciones

I1 = 17.35 mA
 
I2 = 16.87 mA

I3 = 3.89 mA

Calculamos voltaje de R5 con ley de ohm

V = I/R = 3.89/1 = 3.89V

Voltaje y corriente de R5 es

I3 = 3.89

VR5 = 3.89

Para encontrar el volatje de Thévenin lo primero que se va a hacer es eliminar R5

![image](https://user-images.githubusercontent.com/94011974/177988889-30449793-a366-4fb4-a8d5-f0f9bfee7846.png)

Se va a usar las ecuciones del analiss de mallas, tomando en cuando que solo va a existir dos mallas ya que en R5 caen 0V porque no hay corriente, entonces esta resistencia no va a afectar los calculos

Ecuacion 1 

-12 + 0.56(I1) + 4.7(I1-I2) = 0

Ecuacion 2

-2 + 0.33(I2) + 4.7 (I2-I1) = 0

Usando solucionador de ecuaciones hallamos que:

I1 = 15.97

I2 = 15.32

Vthevenin = (15.32)(0.33) = 5.06 V

Para encontrar la resistencia de Thévenin, lo primero que se va a hacer es reemplazar las fuentes de voltajes por sus resistencias internas para posteriormente encontrar las resistencia total.

![image](https://user-images.githubusercontent.com/94011974/177989223-bf84b7ee-2d82-47b8-9902-3dc44fb376dd.png)

Re = ((0.56)(4.7))/0.56+4.7 = 0.500

Re = ((0.500)(0.33))/0.500+0.33 = 0.199 + 0.10 = 0.299 kohm = 299 ohm

Entonces se tiene el voltaje y resistencia de thevenin

VTH = 5.06 V

RTH = 299 ohms

El circuito equivalente.

![image](https://user-images.githubusercontent.com/94011974/177989737-9ece1c8a-5855-47cf-810d-60a0e956c4e4.png)

encontramos voltaje y corrinete en R5

VR5 = (1/(1+0.299))(5.06) = 3.89 V

IR5 = 3.89/1 = 3.89 mA

**5. Respuestas a interrogantes**

5.5.1. Arme el circuito que se muestra en la figura 5.1.

![image](https://user-images.githubusercontent.com/94011974/177990117-e21dac57-8483-4a1a-99d3-2c7e8535a889.png)

5.5.2. Mida el voltaje y la corriente en el resistor R5, anote los resultados en la tabla 5.2.

![image](https://user-images.githubusercontent.com/94011974/177990169-8161b66c-bff0-4b5c-9cf2-ac9737c0a7ce.png)

5.5.3. Desconecte el resistor R5 y mida el voltaje en el circuito abierto. Anote el valor medido en la tabla 5.1.

![image](https://user-images.githubusercontent.com/94011974/177990209-34a040be-7ce2-4c43-9e50-5c1b61e288a7.png)

5.5.4. Anule el efecto de las fuentes de alimentación. Desconecte R5 y desde el circuito abierto resultante mida la resistencia equivalente. Anote el valor medido en la tabla 5.1.

![image](https://user-images.githubusercontent.com/94011974/177990224-f3436b07-cf2a-4bcd-b9ad-6c30d9566f33.png)

5.5.5. Implemente el circuito equivalente de Thévenin, agregue el resistor R5 y mida la corriente y el voltaje en el mismo, anote los resultados en la tabla 5.2.

Tabla 5.1. Valores del Circuito Equivalente de Thévenin

![image](https://user-images.githubusercontent.com/94011974/177990309-310d3816-3343-47b4-8d79-16e7d5380cd8.png)

Tabla 5.2. Comprobación del Teorema de Thévenin.

![image](https://user-images.githubusercontent.com/94011974/177990337-99a145a8-d638-46c5-9f7f-4aaadd1c7e8b.png)

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
