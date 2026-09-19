1. Configurar el Backend

El Backend está desarrollado con FastAPI y contiene el modelo de Machine Learning.

Posicionamiento

Desde la carpeta principal:

Prediccion_Vivienda\Modelos_ML\RegresionLineal

entrar a back:

cd back

La terminal debe quedar ubicada en:

Prediccion_Vivienda\Modelos_ML\RegresionLineal\back
Crear el entorno virtual

Estando dentro de back:

python -m venv venv
Activar el entorno virtual

En Windows:

.\venv\Scripts\Activate.ps1
Instalar las dependencias

Estando todavía dentro de:

Prediccion_Vivienda\Modelos_ML\RegresionLineal\back

ejecutar:

pip install -r requirements.txt
Iniciar el Backend

Ejecutar:

python -m uvicorn main:app --reload --port 8001

El Backend quedará funcionando en:

http://127.0.0.1:8001/

La documentación de la API estará disponible en:

http://127.0.0.1:8001/docs

Mantener esta terminal abierta mientras se utiliza el proyecto.



2. Configurar el Frontend

El Frontend está desarrollado con Django.

Para iniciar el Frontend se debe abrir una segunda terminal, sin cerrar la terminal donde está funcionando el Backend.

Posicionamiento

En la segunda terminal, ubicarse en la carpeta principal:

Prediccion_Vivienda\Modelos_ML\RegresionLineal

Entrar a Front:

cd Front

La terminal debe quedar ubicada en:

Prediccion_Vivienda\Modelos_ML\RegresionLineal\Front
Crear el entorno virtual

Estando dentro de Front:

python -m venv venv
Activar el entorno virtual
.\venv\Scripts\Activate.ps1
Instalar las dependencias

Si dentro de Front existe un archivo requirements.txt, ejecutar:

pip install -r requirements.txt
Realizar las migraciones

Estando ubicado en:

Prediccion_Vivienda\Modelos_ML\RegresionLineal\Front

ejecutar:

python manage.py makemigrations

Después:

python manage.py migrate
Iniciar el Frontend

Ejecutar:

python manage.py runserver 8000

El Frontend estará disponible en:

http://127.0.0.1:8000/

Mantener esta segunda terminal abierta mientras se utiliza el proyecto.
