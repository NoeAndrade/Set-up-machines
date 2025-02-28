Steps:
1.- Configuración e instalación de Sistema operativo
- 250 GB root (tamaño amplio por toda la intalación de software que se require)
- 8 GB swap( la mitad de la memoria RAM de la máquina)
- 2 GB EFI
- 1 TB home


2.- Instalación de VIM
    

3.- Instalar anaconda desde: https://www.anaconda.com/products/navigator

4.- Instalación de Hoomd: 
Para Instalar hoomd con el nombre de la version de hoomd:
https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html
ejemplo:
```
conda create --name hoomd_2.9.6  (se instalara la versión 2.9.6)
```
Una vez creado el ambiente se activa con:
```
conda activate hoomd_2.9.6
```

Una vez activado el ambiente hay que instalar hoomd:
(instalación CPU)
```
conda install hoomd=2.9.6 
```
(instalación GPU)
Primero se rastrean las versiones de hoomd disponibles en conda-forge
conda search hoomd
Selecciona la que tenga el nombre de version 2.9.6 con gpu y la última versión de python que para este caso es la 3.9,ejemplo
```
conda install  hoomd="2.9.6 gpu_py39he2a7f1f_1"
```
Adicionalmente se tiene que instalar las otras librerias de python:
- matplotlib
- pandas
- numpy
- freud
- gsd

5.- Instalación de IDE
  Puedes ocupar VS Code: https://code.visualstudio.com/
  Puedes ocupar jupyter-lab: 
```
  pip install jupyterlab
```
  
