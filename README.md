# Lab-4---API

## Correr la aplicacion

Para correr la aplicacion se debe: 

1. Hhacer un git clone del repositorio
2. Abrir la aplicacion en un IDE (Preferiblemente Visual Studio Code)
3. En la consola (terminal) usar el comando ' uvicorn main:app --reload '
4. Entrar a ' http://127.0.0.1:8000/docs ' desde el navegador

Podrá ver ejemplos de como correr la aplicación, si algún modelo está generando un error (puntuaciones muy bajas), puede que sea un modelo entrenado desde la API. Por lo tanto, se recomienda fuertemeente primero ejecutar los archivos '.ipynb' que se encuentran en la carpeta de Pipeline.

Adicionalmente se puede explorar el API sin necesidad de entrar a docs. En el informe se encuentran ejemplos de como consumir los endpoints.

a.	predictModel{i} : predice un solo resultado, se espera una entrada JSON, retorna los admission points. 

b.	predictionsModel{i} : Predice uno o más resultados, se espera una entrada JSON, retorna una lista de admission points.

c.	scoreModel{i} : retorna el valor de predicción (Explained Variance Score) y valor absoluto medio (MAE) del modelo {i}.

d.	trainModel1{i} : se espera una entrada de JSON con valores para entrenar el modelo, retorna el valor de predicción (Explained           Variance Score) y valor absoluto medio (MAE) del modelo {i}.

Las {i}, representan valores de 1 a 3 (uno para cada modelo), se debe replazar el simbilo por el del modelo que se desea observar. 
