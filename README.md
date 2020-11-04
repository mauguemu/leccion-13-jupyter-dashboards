# Jupyter Dashboards

El repositorio correspondiente a esta lección está disponible en [https://github.com/tpb708-programacionsig-2020/leccion-13-jupyter-dashboards/](https://github.com/tpb708-programacionsig-2020/leccion-13-jupyter-dashboards/). Se recomienda bifurcarlo a su cuenta en GitHub.

## Recursos
- Sitio web de Jupyter Dashboards: [Jupyter Dashboards Layout Extension](https://jupyter-dashboards-layout.readthedocs.io/)

## Notebooks
- [Jupyter Dashboards](https://github.com/tpb708-programacionsig-2020/leccion-13-jupyter-dashboards/blob/master/jupyter-dashboards.ipynb)

## Creación de un ambiente Conda y clonación del repositorio
Ejecute estos comandos desde la línea de comandos de Anaconda, en el directorio en el que desea almacenar el repositorio clonado.
```shell
# Actualización de Conda
conda update -n base -c defaults conda

# Creación del ambiente
conda create -n leccion-13

# Activación del ambiente
conda activate leccion-13

# Instalación de módulos
# GeoPandas, Jupyter, Git
conda config --env --add channels conda-forge
conda config --env --set channel_priority strict
conda install python=3 geopandas matplotlib descartes seaborn folium jupyter jupyter_dashboards git

# Clonación del repositorio (debe sustituir la palabra "usuario" por su nombre de usuario en GitHub)
git clone https://github.com/usuario/leccion-13-jupyter-dashboards.git
cd leccion-13-jupyter-dashboards

# Ejecución del Jupyter Notebook
jupyter notebook

# Actualización del repositorio y de los archivos GeoJSON generados
git add .
git commit -m "Actualizar notebook"
git push

# Desactivación del ambiente Conda
conda deactivate
```
