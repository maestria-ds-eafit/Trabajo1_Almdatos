# Trabajo 1 - Almacenamiento y recuperación de la información

## Integrantes

* David Armendáriz
* Camilo Vélez
* Sebastián Ávila
* David López

## Prerrequisitos

* Instalar Pyenv (Seguir las instrucciones de <https://github.com/pyenv/pyenv>. Nota: no hay Pyenv para Windows. Se recomienda usar WSL (Windows Subsystem for Linux). También tener en cuenta las dependencias de sistemas que hay que instalar antes de instalar cualquier versión de Python en <https://github.com/pyenv/pyenv/wiki>)
* Ejecutar `pyenv local` para verificar la versión local utilizada de Python e instalarla. Por ejemplo `pyenv install 3.11.4`.
* Una vez que se esté usando la versión local, actualizar pip (`pip install --upgrade pip`) para luego instalar Pipenv.
* Instalar Pipenv (`pip install pipenv`)
* Instalar dependencies/crear ambiente virtual (pipenv install)

## Cómo instalar nuevas dependencias

Por ejemplo si se quiere instalar Pandas, hacerlo mediante el comando `pipenv install pandas`.

## Utilización de variables de entorno

Para utilizar variables de entorno para manejar credenciales de AWS o Azure, copiar el archivo `.env.template` y renombrarlo como `.env`.

```terminal
cp .env.template .env
```

El archivo `.env` está en el `.gitignore` así que no se subirá al repositorio. En este archivo se pueden agregar las variables de entorno que se necesiten de manera segura.

## Contenido

* `Arquitectura BATCH en AWS y Azure - Proyecto 1.pdf`: documento entregable para el proyecto
* `ExtractData.ipynb`: el script de Python que permite extraer data del IDEAM y subirla a AWS S3 y Azure Blob Storage.
* `ETL_raw_to_trusted_IDEAM.ipynb`: script que permite transformar la data de la zona raw a la zona trusted en AWS EMR.
* `EDA_Hist_Data.ipynb`: script para hacer análisis exploratorio más profundo de la data histórica.
* `SQL_Scripts_AWS/*`: scripts usados en Redshift.
* `SQL_Scripts_Azure/*`: scripts usados en Azure Synapse.
