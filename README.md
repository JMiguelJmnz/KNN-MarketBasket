# KNN y Market Basket

Analisis de agrupacion por K nearest neighbors y de patrones de consumo por Market basket aplicada a un conjunto de datos de caracteristicas de vino

Cargamos la información inicial
<br>![image](https://github.com/user-attachments/assets/e648788d-2966-40c7-a672-29e8e402fc02)

Definimos la muestra que queremos evaluar y la cantidad de vecinos que utilizaremos
<br>![image](https://github.com/user-attachments/assets/497f2f8e-ecf4-4433-b546-60aec906cc12)

Ejecutamos el algoritmo KNN lo que nos proporciona los indices de los vinos mas cercanos
<br>![image](https://github.com/user-attachments/assets/83a26195-7622-40b8-8b90-94a51411a60f)

Imprimimos la información
<br>![image](https://github.com/user-attachments/assets/2d8d98bc-498f-4e8a-b8a7-59f7a0c34648)

Convertimos a dataframe para visualizar de mejor forma la informacion
<br>![image](https://github.com/user-attachments/assets/1ad162ee-5017-47f3-aff7-4f496320c98a)

Los vecinos más cercanos son
<br>![image](https://github.com/user-attachments/assets/06647db0-049b-4fbd-a9b0-d1bbaf958e4a)

Utilizando la función describe podemos obtener el promedio de la información que queremos saber
<br>![image](https://github.com/user-attachments/assets/45e3e284-0d73-4c12-9b85-94e8cad085a0)

***Conclusion:***
<br>El promedio de alcohol de los 5 vinos más cercanos es de 13.392% tomando en cuenta sus valores individuales de 13.56, 14.06, 13.05, 12.93, 13.36

***Análisis de lista de compras con Market Basket***
<br>Cargamos la información a analizar
<br>![image](https://github.com/user-attachments/assets/9519e652-f876-44f1-9a80-97dbf5b91b11)

Filtramos de base binaria para realizar el análisis
<br>![image](https://github.com/user-attachments/assets/dfd65474-ca47-4686-bece-5f3902748473)

Aplicamos el algoritmo a priori y analizamos con soporte de 3%
<br>![image](https://github.com/user-attachments/assets/012a9d37-c4e7-4ceb-8918-8504455e1a4d)
<br>![image](https://github.com/user-attachments/assets/f6ba6a3e-18d1-4e9b-abcc-8651d979e79a)

Con las reglas de asociación evaluamos segun confianza y lift
<br>![image](https://github.com/user-attachments/assets/985b059b-1dbb-4e1c-acf1-9b8182899ce1)
<br>![image](https://github.com/user-attachments/assets/06b645d2-7282-4b4f-b07c-0dea7b317b17)

Obtenemos bastantes resultados en las dos categorías y de forma agrupada
<br>![image](https://github.com/user-attachments/assets/84ccfa89-e711-4fd8-982f-5fd8e1f81b8b)
<br>![image](https://github.com/user-attachments/assets/c80c2bba-e6f3-4756-a27b-68e1d0cae6af)

Obtenemos que los artículos comprados juntos con mayor frecuencia son el aceite de oliva y el bistec con una confianza de 100% y lift de 11 Seguido, los articulos comprados juntos 
 habitualmente son las manzanas con el espárrago, queso y papas, el vino si se compran bananas, espárrago si se compra salsa y ketchup si se compran alitas de pollo; con 100% de confianza y lift de 5.5, lo que muestra una correlación bastante fuerte, existen más valores con correlación fuerte pero esto nos da un insight de en donde podemos enfocarnos inicialmente para tomar una mayor ventaja en cuanto a la aplicación de promociones o acomodo de los artículos en la tienda.
