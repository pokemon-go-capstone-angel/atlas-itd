# Pokémon data capstone -  Atlas
Ángel Francisco Hernández Valdez - A00839859
Santiago Torres Torres Landa - A00573376


FECHA: 06 de Noviembre de 2026

Repositorio inicial para una exploración reproducible de datos públicos de Pokémon.

## Pregunta del proyecto

¿Cómo cambia la distribución de tipos de Pokémon entre generaciones en la Pokédex pública, y qué tipos aparecen con mayor frecuencia?

## Audiencia

Estudiantes y lectores que quieran entender, con un análisis descriptivo sencillo, cómo se organiza la información de la Pokédex.

## Fuente de datos

Usaremos registros públicos de la Pokédex disponibles en https://pokeapi.co/, una API mantenida por la comunidad. Antes de analizar, registraremos la fecha de consulta, los campos utilizados, la licencia, el método de extracción y las transformaciones. No usaremos datos privados ni telemetría de jugadores de Pokémon GO.

## Resultado esperado

Un notebook reproducible con tablas y gráficas descriptivas por generación y tipo, más un breve reporte que explique los hallazgos y sus límites.

## Limitación actual

Los registros de la Pokédex describen especies y tipos; no miden apariciones, capturas, popularidad ni comportamiento de jugadores dentro de Pokémon GO. Por eso, el análisis no permitirá sacar conclusiones sobre el uso del juego. Las formas regionales y cambios entre versiones también pueden afectar los conteos. Aún no se ha descargado ni validado un corte de datos.

## Cómo empezar

Se requiere Python 3.12 o posterior. Con Anaconda:

~~~powershell
conda env create -f environment.yml
conda activate pokemon-capstone
jupyter lab
~~~

Con Python y pip:

~~~powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python src/hello_ds.py
~~~

El notebook inicial está en notebooks/01-capstone-question.ipynb. Documenta la fuente y el corte de datos antes de agregar resultados.

## Estructura

~~~text
.github/workflows/  Validación automática del código
assignments/        Evidencias y entregas del proyecto
dashboards/         Documentación para tableros futuros
data/raw/           Datos originales, sin modificar
data/processed/     Datos derivados y documentados
docs/               Alcance, arquitectura, gobierno y operación
notebooks/          Análisis exploratorio reproducible
reports/            Hallazgos y visualizaciones
src/                Código Python reutilizable
~~~

No subas contraseñas, tokens, datos personales ni archivos de datos con licencias incompatibles.
