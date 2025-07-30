
# **TelecomX_parte2_Latam**


## **:bookmark_tabs: Problema**

:chart_with_downwards_trend: Alta tasa de desconexion CHURN de la empresa TelecomX.



## :dart: Objetivos:

:bar_chart: Realizar un Análisis exploratorio de la cancelación de clientes

 :computer: Creación de un modelo predictivo que sea capaz de prever la mayor probabilidad de cancelación de servicios.
 
 :chart_with_upwards_trend: Evaluar el rendimiento de los modelos con métricas.


 
 ## **🛠️ Bibliotecas utilizadas:**
 
⚙️https://scikit-learn.org/stable/

⚙️https://pandas.pydata.org/

⚙️https://seaborn.pydata.org/

⚙️https://matplotlib.org/


### :file_folder: Estrategias para la Predicción de Cancelación (Churn) 

La Empresa Telecom X presenta una tasa de cancelación del 26.5%  con este análisis exploratorio se creó un modelo predictivo capaz de detectar los factores que están influyendo en los clientes.


Para realizar el análisis exploratorio se seccionaron las columnas que contiene la base de datos con la finalidad de entender el uso e impacto de cada concepto.


|Productos_disponibles | Protección_cliente | Soporte_cliente |
| :---         |     :---:      |          ---: |
| PhoneService   | OnlineSecurity     | TechSupport    |
| MultipleLinesse     | OnlineBackup       | Contract      |
| InternetService     | DeviceProtection       | Churn      |
| StreamingTV     |        |      |
| StreamingMovies     |        |       |


datos_personales_cliente | 
| :---         |          
| customerID   |    
| customer.gender    |
| customer.SeniorCitizen   |
| customer.Partner    |
| customer.Dependents    |
| customer.tenure   |
| PaperlessBilling    |
| PaymentMethod    |
| Charges.Monthly    |
| Charges.Total    |
| daily_accounts    |




Se detectan variables que no tienen un impacto significativamente en la cancelación.
Como es el caso de:

•	customerID

•	customer.gender

•	customer.SeniorCitizen

•	customer.Partner

•	customer.Dependents


Construyendo los modelos predictivos, se detecta que el modelo de árbol de decisión indica una alta precisión y eso nos da un indicativo respecto a que se debe ajustar el modelo para que generalice bien los datos.

Se entrena el modelo utilizando Algoritmos de aprendizaje supervisado como el modelo de árbol de decisión, el modelo RandomForest y el modelo KNN.

Se obtuvo que los parámetros de mayor importancia y ayudan a detectar el motivo por lo que los clientes deciden cancelar son: 

•	El tipo de contrato mes a mes,

•	 Que no tengan seguridad en línea, 

•	Afecta el método de pago en cheque electrónico.


## **:pushpin:Estrategia para minimizar el porcentaje de cancelación**


1.	Se propone incentivar a los clientes que cambien su periodo a contrato trimestral o semestral
 Para lograr este cambio se sugiere agregue un plazo de 3 meses y 6 meses para que conozcan los productos/servicios de la empresa y después de ese plazo ellos decidan extender su plazo o continuar con este periodo y esto ayudaría a perder menos tiempo en renovaciones continuas.

2.	Se propone implementar la seguridad de la información del cliente, ya que es muy sensible a malas prácticas cibernéticas.
Esto impactara en brindarle mayor confianza al cliente blindando su seguridad.

3.	Se propone que mediante una aplicación de pago se tenga este filtro predeterminado para que el usuario ya no tenga que realizar doble transacción.
   
4.	También se propone agregar un método de pago digital con otro tipo de pago (crédito, debito etc)
Esto ayudaría a que el cliente al tener más opciones del método de pago no tenga que movilizarse o complicarse con su facturación.

