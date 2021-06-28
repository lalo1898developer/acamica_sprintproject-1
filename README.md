# acamica_sprintproject-1

## Instalación de Entorno
Para poder tener Python en tu computadora y gestionar las dependiencias de una forma más sencilla deberas instalar Miniconda.

__[Aqui](https://docs.conda.io/en/latest/miniconda.html) te dejo su link con la lista de instaladores__

- Descarga el instalador para la distribución de tu computador
- Ejecuta el instalador
- Para verificar que tienes instalado todo correctamente, en la consola ejecuta lo siguiente:
    - `python --version`
    - `conda --version`
- Creamos y activamos un ambiente virtual con conda, ejecutamos los siguiente en la consola:
    - `conda create --name acamica1`
    - `conda activate acamica1`

## Instalación de dependencias
Instalaremos todas las dependicas que requiere el proyecto.

- Actualizamos el repositorio de dependencias de conda, ejecuta en la consola:
    - `conda update -n base -c defaults conda`
- Instalamos las dependencias, ejecuta en la consola:
    - `conda install jupyter notebook jupyterlab`
    - `conda install numpy pandas matplotlib seaborn scikit-learn`
    - `conda install -c conda-forge pyproj`
    - `conda install -c conda-forge geopandas`
    - `conda install -c conda-forge geoplot`
    - `conda install shapely fiona rtree`
    - `conda install ipykernel`
- Ligamos nuestro ambiente virtual con uno de JupyterLab, ejecuta en la consola:
    - `ipython kernel install --user --name=acamica1`

## Ejecución del proyecto
Todo se realizara dentro de JupyterLab, para eso debemos levantar el servidor, ejecutar en la consola:
- `jupyter lab`