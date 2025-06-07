# Alura_Teleconx_LATAM

## **Contexto**
Has sido contratado como asistente de análisis de datos en Telecom X y formarás parte del proyecto "Churn de Clientes". La empresa enfrenta una alta tasa de cancelaciones y necesita comprender los factores que llevan a la pérdida de clientes.

## **Limpieza y Tratamiento de Datos**
1. Se realizó la correcta transformación del archivo JSON a un DataFrame de pandas, utilizando el método pd.json_normalize, para ajustar las columnas anidadas.
2. Se eliminaron las columnas 'customer', 'phone', 'internet' y 'account', y se agregaron las columnas ya mencionadas, pero con los datos convertidos en DataFrame.
3. Se verificó la existencia de valores nulos, en este caso no se encontró ninguno.
4. Se corrigieron los nombres de las columnas, se trataron los valores vacíos y se convirtieron las variables categóricas a valores numéricos, como por ejemplo, 'Yes': 1, 'No': 0, 'No phone service': 2, y se eliminaron las filas donde el registro de 'Churn' estaba vacío.
## **Análisis Exploratorio de Datos**
### **Variables Categóricas**
![Image](https://github.com/user-attachments/assets/b36da904-145d-41e9-9221-1f9216ec20c2)

Se observa que no hay mucha relación entre hombres y mujeres y la evasión (Churn).
![Image](https://github.com/user-attachments/assets/33b2f297-34b3-47d3-a193-f6c461099c34)

En la relación entre tipo de contrato, se encontró una relación entre las personas que tienen un tipo de contrato mes a mes y el abandono o evasión (Churn).
![Image](https://github.com/user-attachments/assets/1980e658-b3eb-4932-a723-9f323fa20809)

Muy parecido a lo anterior, se evidencia una clara cantidad de abandono o evasión (Churn) relacionada con el método de pago por factura electrónica.
![Image](https://github.com/user-attachments/assets/8066b208-5e38-4d99-86b2-e4528ca8bdb6)

Se encuentra un alto índice de abandono o evasión (Churn) en los usuarios con fibra óptica
### **Variables Numéricas***
![Image](https://github.com/user-attachments/assets/8621bd70-d473-4709-ae86-e95860abf0e6)

Se evidencia que la gran mayoría de los clientes de la empresa están en un rango de menos de 1000 USD de gastos anuales, y las personas que abandonan o evaden (Churn), en su gran mayoría están en este rango, aunque la mediana de los que no evaden es mayor que la de las personas que evaden.
![Image](https://github.com/user-attachments/assets/31141db7-f85c-4002-aa0d-8f41c291045c)

El tiempo en el que se encuentran las personas que abandonan o evaden (Churn) se sitúa en una tenencia (Tenure) de su contrato igual o menor a 30 meses. La media de las personas que no evaden es cercana a 40 meses de tenencia, mientras que la media de los que abandonan es alrededor de 12 meses de tenencia.
## **Conclusiones e Insights**
1. El grueso de los clientes se encuentra entre 200 y 2000 USD de gasto anual.
2. La inmensa mayoría de las personas que hacen Churn están con contratos menores de 30 meses.
3. Hay una fuerte relación entre el internet por fibra óptica y el abandono o evasión (Churn).
4. Hay una fuerte relación entre la factura electrónica y el Churn.
5. Hay evidencia de relación entre el contrato mes a mes y el abandono o evasión (Churn).
6. No se encuentra una relación entre el Churn y el género.
## **Recomendaciones**
1. Implementar promociones o campañas como método de fidelización para las personas con pocos meses de contrato.
2. Ofrecer promociones a las personas con gastos entre 200 y 2000 USD.
3. Revisar la calidad, atención al cliente y otros factores en el servicio de fibra óptica.
4. Dar beneficios a los usuarios que paguen por pago electrónico.
5. Ofrecer promociones cortas a los usuarios con contratos mes a mes.
