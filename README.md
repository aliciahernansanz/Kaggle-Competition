# Kaggle-Competition





 
### Transformación y Limpieza 🧹
 
🔗 Concatenamos el archivo de Salario y el Testeo para aplicar los cambios simultáneamente a ambos archivos.
💶 Definimos la variable ‘y’ = ‘salary_in_usd’
❌ Eliminamos las columnas de salary y salary_currency
✂️ En las columnas ‘company_location’ y ‘employee_residence’ agrupamos los paises con menos de 5 registros como ‘other’.


### Preparación y aplicación modelo predictivo 

- Aplicamos Get Dummies a todas las columnas ‘object’.
- Normalizamos el dato aplicando StandarScaler 
- Separamos el DataFrame en Salario y en Testeo.
- Entrenamos el modelo y usamos LazyRegressor para encontrar el modelo con el RMSE más bajo.
- Predecimos con GammaRegressor.

### Observaciones

- Cuantos más cambios en algunas columnas o cuando eliminamos ciertas columnas, el error crece.
- El RMSE que me da con en el la predicción en Jupyter decrece al subirlo a Kaggle.