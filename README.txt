PROYECTO: SIMULACIÓN DE CONCENTRACIÓN INDUSTRIAL MEDIANTE MONTE CARLO

DESCRIPCIÓN
-----------
Aplicación web desarrollada en Python y Streamlit para analizar la concentración
industrial mediante simulaciones de Monte Carlo.

La aplicación permite calcular los siguientes indicadores:

- Ratio de Concentración (CR_k)
- Índice de Herfindahl-Hirschman (IHH)
- Índice de Dominancia (ID)
- Índice de Entropía (IE)

También permite generar o ingresar un caso particular, comparar su resultado
con una distribución de simulaciones Monte Carlo y evaluar el nivel de
concentración mediante un módulo interactivo.

REQUISITOS
----------
- Python 3.9 o superior
- pip

INSTALACIÓN
-----------
1. Descargar o clonar el proyecto.

2. Abrir una terminal dentro de la carpeta principal del proyecto.

3. Instalar las dependencias ejecutando:

   pip install -r requirements.txt

EJECUCIÓN LOCAL
---------------
Una vez instaladas las dependencias, ejecutar:

   streamlit run app.py

Si el archivo principal tiene otro nombre, reemplazar "app.py" por el nombre
correspondiente.

La aplicación se abrirá automáticamente en el navegador.

Si no se abre automáticamente, acceder desde el navegador a:

   http://localhost:8501

USO DE LA APLICACIÓN
--------------------
1. Seleccionar el indicador de concentración.

2. Definir el número de empresas (N), entre 2 y 100.

3. Definir el número de iteraciones de Monte Carlo.
   El valor predeterminado es 1.000 y el máximo permitido es 100.000.

4. Para CR_k, seleccionar el número de empresas consideradas en el cálculo.

5. Generar un caso particular aleatorio o ingresar manualmente las cuotas
   de mercado.

6. La aplicación valida que las cuotas sean válidas y que sumen 1.

7. Ejecutar la simulación de Monte Carlo.

8. Revisar la distribución simulada, el valor del caso particular y su
   percentil.

9. Utilizar el módulo evaluador para clasificar el nivel de concentración
   como Baja, Moderada o Alta.

ADVERTENCIA DE CARGA COMPUTACIONAL
-----------------------------------
Un mayor número de iteraciones aumenta la precisión de la simulación, pero
también incrementa el consumo de CPU y memoria y puede aumentar el tiempo
de respuesta de la aplicación.

Para una ejecución rápida se recomienda comenzar con 1.000 iteraciones.
