PROGRAMACIÓN DE APLICACIONES SIG
TAREA 02 B
ELABORADO POR: GEANCARLO MELÉNDEZ SALAZAR
INSTALACIÓN DE FUENTES PRIMARIAS
En el siguiente apartado se colocará los comandos para la instalación de fuentes primarias


# Instalación de libspatialindex-dev y rtree
# Debe realizarse antes de la instalación de geopandas
!apt install libspatialindex-dev
!pip install --upgrade rtree

# Instalación de geopandas y otros módulos módulos
!pip install --upgrade geopandas
!pip install --upgrade pyshp
!pip install --upgrade shapely
!pip install --upgrade mapclassify
!pip install --upgrade descartes
!pip install --sidetable
     
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  libspatialindex-c6 libspatialindex6
The following NEW packages will be installed:
  libspatialindex-c6 libspatialindex-dev libspatialindex6
0 upgraded, 3 newly installed, 0 to remove and 19 not upgraded.
Need to get 319 kB of archives.
After this operation, 1,416 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu jammy/universe amd64 libspatialindex6 amd64 1.9.3-2 [247 kB]
Get:2 http://archive.ubuntu.com/ubuntu jammy/universe amd64 libspatialindex-c6 amd64 1.9.3-2 [55.8 kB]
Get:3 http://archive.ubuntu.com/ubuntu jammy/universe amd64 libspatialindex-dev amd64 1.9.3-2 [16.0 kB]
Fetched 319 kB in 1s (538 kB/s)
Selecting previously unselected package libspatialindex6:amd64.
(Reading database ... 120874 files and directories currently installed.)
Preparing to unpack .../libspatialindex6_1.9.3-2_amd64.deb ...
Unpacking libspatialindex6:amd64 (1.9.3-2) ...
Selecting previously unselected package libspatialindex-c6:amd64.
Preparing to unpack .../libspatialindex-c6_1.9.3-2_amd64.deb ...
Unpacking libspatialindex-c6:amd64 (1.9.3-2) ...
Selecting previously unselected package libspatialindex-dev:amd64.
Preparing to unpack .../libspatialindex-dev_1.9.3-2_amd64.deb ...
Unpacking libspatialindex-dev:amd64 (1.9.3-2) ...
Setting up libspatialindex6:amd64 (1.9.3-2) ...
Setting up libspatialindex-c6:amd64 (1.9.3-2) ...
Setting up libspatialindex-dev:amd64 (1.9.3-2) ...
Processing triggers for libc-bin (2.35-0ubuntu3.1) ...
/sbin/ldconfig.real: /usr/local/lib/libtbbbind.so.3 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libtbbbind_2_0.so.3 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libtbb.so.12 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libtbbmalloc.so.2 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libtbbmalloc_proxy.so.2 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libtbbbind_2_5.so.3 is not a symbolic link

Collecting rtree
  Downloading Rtree-1.1.0-py3-none-manylinux2014_x86_64.manylinux_2_17_x86_64.whl (488 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 488.6/488.6 kB 6.7 MB/s eta 0:00:00
Installing collected packages: rtree
Successfully installed rtree-1.1.0
Requirement already satisfied: geopandas in /usr/local/lib/python3.10/dist-packages (0.13.2)
Collecting geopandas
  Downloading geopandas-0.14.0-py3-none-any.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 7.7 MB/s eta 0:00:00
Requirement already satisfied: fiona>=1.8.21 in /usr/local/lib/python3.10/dist-packages (from geopandas) (1.9.5)
Requirement already satisfied: packaging in /usr/local/lib/python3.10/dist-packages (from geopandas) (23.2)
Requirement already satisfied: pandas>=1.4.0 in /usr/local/lib/python3.10/dist-packages (from geopandas) (1.5.3)
Requirement already satisfied: pyproj>=3.3.0 in /usr/local/lib/python3.10/dist-packages (from geopandas) (3.6.1)
Requirement already satisfied: shapely>=1.8.0 in /usr/local/lib/python3.10/dist-packages (from geopandas) (2.0.2)
Requirement already satisfied: attrs>=19.2.0 in /usr/local/lib/python3.10/dist-packages (from fiona>=1.8.21->geopandas) (23.1.0)
Requirement already satisfied: certifi in /usr/local/lib/python3.10/dist-packages (from fiona>=1.8.21->geopandas) (2023.7.22)
Requirement already satisfied: click~=8.0 in /usr/local/lib/python3.10/dist-packages (from fiona>=1.8.21->geopandas) (8.1.7)
Requirement already satisfied: click-plugins>=1.0 in /usr/local/lib/python3.10/dist-packages (from fiona>=1.8.21->geopandas) (1.1.1)
Requirement already satisfied: cligj>=0.5 in /usr/local/lib/python3.10/dist-packages (from fiona>=1.8.21->geopandas) (0.7.2)
Requirement already satisfied: six in /usr/local/lib/python3.10/dist-packages (from fiona>=1.8.21->geopandas) (1.16.0)
Requirement already satisfied: setuptools in /usr/local/lib/python3.10/dist-packages (from fiona>=1.8.21->geopandas) (67.7.2)
Requirement already satisfied: python-dateutil>=2.8.1 in /usr/local/lib/python3.10/dist-packages (from pandas>=1.4.0->geopandas) (2.8.2)
Requirement already satisfied: pytz>=2020.1 in /usr/local/lib/python3.10/dist-packages (from pandas>=1.4.0->geopandas) (2023.3.post1)
Requirement already satisfied: numpy>=1.21.0 in /usr/local/lib/python3.10/dist-packages (from pandas>=1.4.0->geopandas) (1.23.5)
Installing collected packages: geopandas
  Attempting uninstall: geopandas
    Found existing installation: geopandas 0.13.2
    Uninstalling geopandas-0.13.2:
      Successfully uninstalled geopandas-0.13.2
ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
lida 0.0.10 requires fastapi, which is not installed.
lida 0.0.10 requires kaleido, which is not installed.
lida 0.0.10 requires python-multipart, which is not installed.
lida 0.0.10 requires uvicorn, which is not installed.
Successfully installed geopandas-0.14.0
Requirement already satisfied: pyshp in /usr/local/lib/python3.10/dist-packages (2.3.1)
Requirement already satisfied: shapely in /usr/local/lib/python3.10/dist-packages (2.0.2)
Requirement already satisfied: numpy>=1.14 in /usr/local/lib/python3.10/dist-packages (from shapely) (1.23.5)
Collecting mapclassify
  Downloading mapclassify-2.6.1-py3-none-any.whl (38 kB)
Requirement already satisfied: networkx>=2.7 in /usr/local/lib/python3.10/dist-packages (from mapclassify) (3.2.1)
Requirement already satisfied: numpy>=1.23 in /usr/local/lib/python3.10/dist-packages (from mapclassify) (1.23.5)
Requirement already satisfied: pandas!=1.5.0,>=1.4 in /usr/local/lib/python3.10/dist-packages (from mapclassify) (1.5.3)
Requirement already satisfied: scikit-learn>=1.0 in /usr/local/lib/python3.10/dist-packages (from mapclassify) (1.2.2)
Requirement already satisfied: scipy>=1.8 in /usr/local/lib/python3.10/dist-packages (from mapclassify) (1.11.3)
Requirement already satisfied: python-dateutil>=2.8.1 in /usr/local/lib/python3.10/dist-packages (from pandas!=1.5.0,>=1.4->mapclassify) (2.8.2)
Requirement already satisfied: pytz>=2020.1 in /usr/local/lib/python3.10/dist-packages (from pandas!=1.5.0,>=1.4->mapclassify) (2023.3.post1)
Requirement already satisfied: joblib>=1.1.1 in /usr/local/lib/python3.10/dist-packages (from scikit-learn>=1.0->mapclassify) (1.3.2)
Requirement already satisfied: threadpoolctl>=2.0.0 in /usr/local/lib/python3.10/dist-packages (from scikit-learn>=1.0->mapclassify) (3.2.0)
Requirement already satisfied: six>=1.5 in /usr/local/lib/python3.10/dist-packages (from python-dateutil>=2.8.1->pandas!=1.5.0,>=1.4->mapclassify) (1.16.0)
Installing collected packages: mapclassify
Successfully installed mapclassify-2.6.1
Collecting descartes
  Downloading descartes-1.1.0-py3-none-any.whl (5.8 kB)
Requirement already satisfied: matplotlib in /usr/local/lib/python3.10/dist-packages (from descartes) (3.7.1)
Requirement already satisfied: contourpy>=1.0.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (1.2.0)
Requirement already satisfied: cycler>=0.10 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (0.12.1)
Requirement already satisfied: fonttools>=4.22.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (4.44.0)
Requirement already satisfied: kiwisolver>=1.0.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (1.4.5)
Requirement already satisfied: numpy>=1.20 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (1.23.5)
Requirement already satisfied: packaging>=20.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (23.2)
Requirement already satisfied: pillow>=6.2.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (9.4.0)
Requirement already satisfied: pyparsing>=2.3.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (3.1.1)
Requirement already satisfied: python-dateutil>=2.7 in /usr/local/lib/python3.10/dist-packages (from matplotlib->descartes) (2.8.2)
Requirement already satisfied: six>=1.5 in /usr/local/lib/python3.10/dist-packages (from python-dateutil>=2.7->matplotlib->descartes) (1.16.0)
Installing collected packages: descartes
Successfully installed descartes-1.1.0

Usage:   
  pip3 install [options] <requirement specifier> [package-index-options] ...
  pip3 install [options] -r <requirements file> [package-index-options] ...
  pip3 install [options] [-e] <vcs project url> ...
  pip3 install [options] [-e] <local project path> ...
  pip3 install [options] <archive url/path> ...

no such option: --sidetable
CARGAS
En el siguiente apartado se colocará los comandos para la importación de insumos primarios

CARGA DE PAQUETES
Se importarán los siguientes insumos:

pandas
geopandas
plotly.express
matplotlib.pyplot
seaborn
numpy

import pandas as pd
     

import geopandas as gpd
     

# Versión de geopandas
gpd.__version__
     
'0.13.2'

# Carga de plotly express, matplotlib y seaborn
import plotly.express as px
import matplotlib.pyplot as plt
import seaborn as sns


# Carga de plotly figure factory,
# para tipos adicionales de gráficos
import plotly.figure_factory as ff

# Carga de numpy para sumatorias
import numpy as np
plt.style.use('_mpl-gallery-nogrid')
     
CARGA DE DATOS
Se cargarán las siguientas capas/tablas que previamente fueron cargadas al Google Drive:

catastro
plan regulador
zonas homogéneas
patentados
patentes
barrios
Las capas anteriores son propiedad de la Municipalidad de Puntarenas y son utilizadas solo con fines académicos.


from google.colab import drive
drive.mount('/content/drive')
     
Mounted at /content/drive
VISUALIZACIÓN DE DATOS
La siguiente es una visualización tanto en tablas como en gráficos de los datos en el que se identifican sus características generales.

CATASTRO

catastro = gpd.read_file("/content/drive/MyDrive/programacion/catastro.gpkg")
     

catastro
     
identifica	finca	plano	bloque	predio	ID	codigo	geometry
0	6010100031940M	0003194	610948172006	143	005	3	u35	MULTIPOLYGON (((412376.650 1103789.226, 412387...
1	601010021048A0	0021048	600112181971	143	003	3	u12	MULTIPOLYGON (((412802.190 1103745.306, 412798...
2	60101000521500	0005215	600017471972	143	004	3	u12	MULTIPOLYGON (((412388.035 1103868.591, 412377...
3	60101P00003100	P000031	600000002023	143	001	3	u12	MULTIPOLYGON (((413684.729 1103717.705, 413544...
4	60101013453600	0134536	608501392003	128	006	3	u13/u14	MULTIPOLYGON (((410969.577 1103867.878, 411035...
...	...	...	...	...	...	...	...	...
3217	60101005665800	0056658	607243701988	001	007	1	u25/u26	MULTIPOLYGON (((406860.832 1103340.078, 406854...
3218	60101005665600	0056656	607326191988	001	008	1	u23	MULTIPOLYGON (((406864.043 1103334.565, 406849...
3219	60101P00755100	P007551	600000002023	001	030	1	u23	MULTIPOLYGON (((406817.406 1103314.138, 406813...
3220	60101000000000	0000000	600000002023	128	001	3	u08/u09	MULTIPOLYGON (((411326.638 1103860.465, 411326...
3221	60101P00902700	P009027	600000002023	031	000	1	u24	MULTIPOLYGON (((407679.797 1103323.414, 407686...
3222 rows × 8 columns


catastro.plot(marker='o', color='#e5e1d5', edgecolor="#cac3ac", markersize=50, figsize=(20, 20))
     
<Axes: >

PLAN REGULADOR

plan = gpd.read_file("/content/drive/MyDrive/programacion/plan.gpkg")
plan
     
BLOQUE	Predios_Es	Nombre	ID	codigo	geometry
0	012	18.0	Zona Residencial Comercial Mixta	1	u21	MULTIPOLYGON (((407185.200 1103064.474, 407198...
1	027	2.0	Zona Residencial Comercial Mixta	1	u21	MULTIPOLYGON (((407574.491 1103063.450, 407622...
2	028	8.0	Zona Comercial Residencial Mixta	1	u18/u19	MULTIPOLYGON (((407662.006 1103067.022, 407667...
3	011	11.0	Zona Residencial Comercial Mixta	1	u21	MULTIPOLYGON (((407036.345 1103083.935, 407036...
4	019	15.0	Zona Residencial Comercial Mixta	1	u21	MULTIPOLYGON (((407299.660 1103070.530, 407309...
...	...	...	...	...	...	...
295	000	0.0	Carreteras Existentes (Zona Vial)	2	u07	MULTIPOLYGON (((407320.303 1103037.726, 407311...
296	073	34.0	Zona Pública Institucional	2	None	MULTIPOLYGON (((408744.794 1103593.941, 408785...
297	073	34.0	Zona Pública Institucional	2	None	MULTIPOLYGON (((408738.126 1103592.692, 408737...
298	000	0.0	Zona de Parques	2	u18/u19	MULTIPOLYGON (((408952.197 1103148.156, 408957...
299	000	0.0	Zona de Parques	3	u12	MULTIPOLYGON (((412719.664 1103721.257, 412724...
300 rows × 6 columns


px.histogram(data_frame=plan,
             x="Nombre",
             color="codigo",
             nbins=15,
             title="Distribución de las categorías de usos del Plan Regulador de la ciudad de Puntarenas")
     

plan.plot(edgecolor='black', facecolor="#e5e1d5", figsize=(20, 20));
     

ZONAS HOMOGÉNEAS

zonas = gpd.read_file("/content/drive/MyDrive/programacion/zonas.gpkg")
zonas
     
NOMBRE_ZON	VALOR	codigo	ID	geometry
0	sector san lucas beach club	190000.0	u22	1	MULTIPOLYGON (((406747.210 1103361.580, 406752...
1	sector barrio del carmen sur	130000.0	u21	1	MULTIPOLYGON (((408094.849 1103291.980, 408095...
2	parque marino del pacifico	100000.0	u17	2	MULTIPOLYGON (((409542.777 1103395.197, 409549...
3	invu - el cocal	35000.0	u07	3	MULTIPOLYGON (((410834.338 1103860.599, 410837...
4	hotel riu - grupo mutual	210000.0	u02	2	MULTIPOLYGON (((408925.062 1103701.023, 408926...
5	municipalidad de puntarenas - escuela de biolo...	160000.0	u20	2	MULTIPOLYGON (((408426.266 1103408.293, 408427...
6	sector incopesca	190000.0	u27	2	MULTIPOLYGON (((408178.295 1103604.005, 408178...
7	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...
8	sector norte barrio el carmen	53000.0	u24	1	MULTIPOLYGON (((408189.734 1103490.446, 408191...
9	sector escuela delia urbina de guevara	160000.0	u28	2	MULTIPOLYGON (((408423.794 1103598.435, 408439...
10	sector playitas sur	185000.0	u05	2	MULTIPOLYGON (((409607.423 1103515.723, 409609...
11	sector colegio nuestra señora de sion	90000.0	u15/u16	3	MULTIPOLYGON (((410406.349 1103599.735, 410406...
12	sector de playa pochote	135000.0	u13/u14	3	MULTIPOLYGON (((410404.563 1103607.654, 410397...
13	barrio la chanchera - ucr	125000.0	u08/u09	3	MULTIPOLYGON (((410695.110 1103950.120, 410710...
14	clinica san rafael - anfiteatro municipal	270000.0	u18/u19	2	MULTIPOLYGON (((408981.838 1103223.956, 408989...
15	terminal de ferry	150000.0	u25/u26	1	MULTIPOLYGON (((406951.760 1103446.500, 406971...
16	barrio el carmen - estadio lito perez	170000.0	u23	1	MULTIPOLYGON (((408216.447 1103366.109, 408217...
17	las playitas	100000.0	u03/u04	2	MULTIPOLYGON (((409314.027 1103537.971, 409314...
18	condominio puerto azul boutique resort & marina	250000.0	u35	3	MULTIPOLYGON (((412574.160 1103831.294, 412573...
19	el cocal	85000.0	u06	3	MULTIPOLYGON (((410404.563 1103607.654, 410393...
20	sector de playa angostura	100000.0	u12	3	MULTIPOLYGON (((412668.430 1103793.000, 412691...
21	crematorio	40000.0	u36	1	MULTIPOLYGON (((407519.536 1103345.010, 407486...

zonas.plot(column="VALOR",
                    legend=True,
                    cmap='OrRd',
                    scheme='quantiles',
                    figsize=(20, 20))
     
<Axes: >


zonas.plot(edgecolor='black', facecolor="#e5e1d5", figsize=(20, 20));
     

PATENTADOS

patentados = pd.read_csv("/content/drive/MyDrive/programacion/patentados.csv", sep=",")
patentados
     
fid	nombre_completo	telefono	cedula
0	1	fundacion desarrollo colegio universitario pun...	87028046	3.006114e+09
1	2	corporaciÃƒÂ³n tyk y tac catÃƒÂ¡logo y ventas ...	26610017	3.102779e+09
2	3	blue riviera and cosociedad de responsabilidad...	83981172	3.102350e+09
3	4	temporalidades iglesia catolica diocesis de p...	26619174	3.010228e+09
4	5	distribuidora apui sociedad de responsabilidad...	88204132	3.102769e+09
...	...	...	...	...
821	822	bluefin sa	61763122	3.101250e+09
822	823	cayuga s.a	84463805	3.101011e+09
823	824	lokale s.a	60454266	3.101859e+09
824	825	rulefa s.a	83351816	3.101207e+09
825	826	promarsa	26613050	3.101761e+09
826 rows × 4 columns


patentados.info()
     
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 826 entries, 0 to 825
Data columns (total 4 columns):
 #   Column           Non-Null Count  Dtype  
---  ------           --------------  -----  
 0   fid              826 non-null    int64  
 1   nombre_completo  826 non-null    object 
 2   telefono         826 non-null    int64  
 3   cedula           826 non-null    float64
dtypes: float64(1), int64(2), object(1)
memory usage: 25.9+ KB

patentados['cedula'] = patentados['cedula'].astype('object');
     

patentados
     
fid	nombre_completo	telefono	cedula
0	1	fundacion desarrollo colegio universitario pun...	87028046	3006114055.0
1	2	corporaciÃƒÂ³n tyk y tac catÃƒÂ¡logo y ventas ...	26610017	3102779250.0
2	3	blue riviera and cosociedad de responsabilidad...	83981172	3102350182.0
3	4	temporalidades iglesia catolica diocesis de p...	26619174	3010228347.0
4	5	distribuidora apui sociedad de responsabilidad...	88204132	3102769129.0
...	...	...	...	...
821	822	bluefin sa	61763122	3101249587.0
822	823	cayuga s.a	84463805	3101011109.0
823	824	lokale s.a	60454266	3101859465.0
824	825	rulefa s.a	83351816	3101206615.0
825	826	promarsa	26613050	3101760526.0
826 rows × 4 columns

PATENTES

patentes = gpd.read_file("/content/drive/MyDrive/programacion/patentes.gpkg")
patentes
     
num_pat	nom_com	tipo_pat	cat_com	licen_lic	finca	cedula	ID	codigo	bloque	geometry
0	2777.0	hotel_c.r._yacht_club	desocupado	comercio	d2	0021048	3101005849	3	u12	143	POINT (412708.706 1103747.239)
1	3317.0	soda_ucr	comercial	comercio	n/a	0134536	601001232	3	u08/u09	128	POINT (411148.703 1103802.039)
2	5279.0	ceviches_del_puerto	ambas	comercio	c	0015277	603340776	3	u12	143	POINT (412883.074 1103723.416)
3	5333.0	carvher_pet	comercial	comercio	n/a	0013227	602540562	3	u08/u09	143	POINT (412164.568 1103823.921)
4	3380.0	encuadernacion_el_cocal	comercial	comercio	n/a	0011710	602190453	3	u08/u09	143	POINT (412033.491 1103822.117)
...	...	...	...	...	...	...	...	...	...	...	...
333	1683.0	hotel_yadran_beach_resort	ambas	servicio	d2	0014969	3101077294	1	u22	003	POINT (406850.610 1103167.059)
334	3818.0	hotel_la_punta	ambas	servicio	e1a	0174660	3101559994	1	u23	001	POINT (406851.985 1103300.416)
335	494.0	bar_restaurante_manglamar	ambas	servicio	c	0180507	601510423	1	u23	002	POINT (406833.861 1103199.381)
336	5752.0	tiki_brunch	ambas	comercio	sd	0176863	601720332	1	u25/u26	001	POINT (406801.429 1103349.859)
337	2947.0	isla_cocos	ambas	comercio	c	0176862	3101283487	1	u25/u26	001	POINT (406789.631 1103344.069)
338 rows × 11 columns


from matplotlib import pyplot as plt
import seaborn as sns
patentes.groupby('cat_com').size().plot(kind='barh', color=sns.palettes.mpl_palette('Dark2'))
plt.gca().spines[['top', 'right',]].set_visible(False),
plt.title("Distribución de la categoría comercial en las patentes del distrito Puntarenas"),
figsize=(100, 100)
     


from matplotlib import pyplot as plt
import seaborn as sns
patentes.groupby('tipo_pat').size().plot(kind='barh', color=sns.palettes.mpl_palette('Dark2'))
plt.gca().spines[['top', 'right',]].set_visible(False)
plt.title("Distribución de tipo de patentes comercial del distrito Puntarenas"),
figsize=(100, 100)
     


from matplotlib import pyplot as plt
import seaborn as sns
figsize = (12, 1.2 * len(patentes['licen_lic'].unique()))
plt.figure(figsize=figsize)
sns.violinplot(patentes, x='ID', y='licen_lic', inner='stick', palette='Dark2')
sns.despine(top=True, right=True, bottom=True, left=True)
plt.title("Distribución de patentes de licores en el distrito Puntarenas por barrios"),
     
(Text(0.5, 1.0, 'Distribución de patentes de licores en el distrito Puntarenas por barrios'),)


patentes.plot(color='#01f761', edgecolor='#450000', figsize=(20, 20), markersize=10)
     
<Axes: >


patentes.info()
     
<class 'geopandas.geodataframe.GeoDataFrame'>
RangeIndex: 338 entries, 0 to 337
Data columns (total 11 columns):
 #   Column     Non-Null Count  Dtype   
---  ------     --------------  -----   
 0   num_pat    338 non-null    float64 
 1   nom_com    338 non-null    object  
 2   tipo_pat   338 non-null    object  
 3   cat_com    338 non-null    object  
 4   licen_lic  338 non-null    object  
 5   finca      338 non-null    object  
 6   cedula     338 non-null    object  
 7   ID         338 non-null    int64   
 8   codigo     338 non-null    object  
 9   bloque     338 non-null    object  
 10  geometry   338 non-null    geometry
dtypes: float64(1), geometry(1), int64(1), object(8)
memory usage: 29.2+ KB
BARRIOS

barrios = gpd.read_file("/content/drive/MyDrive/programacion/barrios.gpkg")
barrios
     
nombre	ID	geometry
0	barrio_el_carmen	1	MULTIPOLYGON (((408104.200 1103019.393, 407780...
1	puntarenas_centro	2	MULTIPOLYGON (((408104.200 1103019.393, 408040...
2	el_cocal	3	MULTIPOLYGON (((409547.121 1103338.226, 409517...

barrios.plot(edgecolor='black', facecolor="none", figsize=(20, 20))
     
<Axes: >

INTEGRACIÓN DE DATOS
Se presentarán uniones de tablas para ligar información interrelacionada que sea de interés para mostrar algún dato en específico.

LOCALES COMERCIALES SEGÚN ZONAS HOMOGENAS

zonas_comercios = zonas.merge(patentes, on='codigo')
     

zonas_comercios
     
NOMBRE_ZON	VALOR	codigo	ID_x	geometry_x	num_pat	nom_com	tipo_pat	cat_com	licen_lic	finca	cedula	ID_y	bloque	geometry_y
0	sector san lucas beach club	190000.0	u22	1	MULTIPOLYGON (((406747.210 1103361.580, 406752...	5255.0	minisuper_y_licorera_parq	ambas	comercio	a	0008269	3101756935	1	027	POINT (407617.611 1103071.312)
1	sector san lucas beach club	190000.0	u22	1	MULTIPOLYGON (((406747.210 1103361.580, 406752...	4695.0	restaurante_el_joron	desocupado	comercio	c	0007931	3101696720	1	026	POINT (407524.161 1103100.528)
2	sector san lucas beach club	190000.0	u22	1	MULTIPOLYGON (((406747.210 1103361.580, 406752...	5293.0	snakeria_grill	comercial	servicio	n/a	0008189	602780515	1	020	POINT (407446.109 1103091.883)
3	sector san lucas beach club	190000.0	u22	1	MULTIPOLYGON (((406747.210 1103361.580, 406752...	1627.0	bar_y_restaurante_mastil	comercial	servicio	c	0076977	602280701	1	020	POINT (407420.909 1103088.542)
4	sector san lucas beach club	190000.0	u22	1	MULTIPOLYGON (((406747.210 1103361.580, 406752...	4516.0	la_ventanita_del_gordo	ambas	comercio	c	0007684	204510194	1	019	POINT (407315.230 1103073.849)
...	...	...	...	...	...	...	...	...	...	...	...	...	...	...	...
333	crematorio	40000.0	u36	1	MULTIPOLYGON (((407519.536 1103345.010, 407486...	1088.0	pescaderia_los_palmareÃ±o	comercial	comercio	n/a	0110528	3101192754	1	007	POINT (407080.468 1103398.969)
334	crematorio	40000.0	u36	1	MULTIPOLYGON (((407519.536 1103345.010, 407486...	3257.0	hielo_mar	comercial	comercio	n/a	0053753	3101658184	1	007	POINT (407151.673 1103406.826)
335	crematorio	40000.0	u36	1	MULTIPOLYGON (((407519.536 1103345.010, 407486...	1113.0	fabrica_de_hielo_los_palm	comercial	comercio	n/a	0ZM0004	3101273673	1	007	POINT (407049.959 1103393.295)
336	crematorio	40000.0	u36	1	MULTIPOLYGON (((407519.536 1103345.010, 407486...	1116.0	suministros_el_barrio_s.a	comercial	comercio	n/a	0128411	3101276507	1	007	POINT (407062.661 1103392.267)
337	crematorio	40000.0	u36	1	MULTIPOLYGON (((407519.536 1103345.010, 407486...	5561.0	exportadora_frumar	comercial	comercio	n/a	0097713	3101096583	1	007	POINT (407231.563 1103406.623)
338 rows × 15 columns


zonas_comercios2 = zonas_comercios[["NOMBRE_ZON", "codigo", "VALOR", "cat_com", "geometry_x"]]
zonas_comercios2
     
NOMBRE_ZON	codigo	VALOR	cat_com	geometry_x
0	sector san lucas beach club	u22	190000.0	comercio	MULTIPOLYGON (((406747.210 1103361.580, 406752...
1	sector san lucas beach club	u22	190000.0	comercio	MULTIPOLYGON (((406747.210 1103361.580, 406752...
2	sector san lucas beach club	u22	190000.0	servicio	MULTIPOLYGON (((406747.210 1103361.580, 406752...
3	sector san lucas beach club	u22	190000.0	servicio	MULTIPOLYGON (((406747.210 1103361.580, 406752...
4	sector san lucas beach club	u22	190000.0	comercio	MULTIPOLYGON (((406747.210 1103361.580, 406752...
...	...	...	...	...	...
333	crematorio	u36	40000.0	comercio	MULTIPOLYGON (((407519.536 1103345.010, 407486...
334	crematorio	u36	40000.0	comercio	MULTIPOLYGON (((407519.536 1103345.010, 407486...
335	crematorio	u36	40000.0	comercio	MULTIPOLYGON (((407519.536 1103345.010, 407486...
336	crematorio	u36	40000.0	comercio	MULTIPOLYGON (((407519.536 1103345.010, 407486...
337	crematorio	u36	40000.0	comercio	MULTIPOLYGON (((407519.536 1103345.010, 407486...
338 rows × 5 columns


zonas_comercios[zonas_comercios["VALOR"] >= 330000]
     
NOMBRE_ZON	VALOR	codigo	ID_x	geometry_x	num_pat	nom_com	tipo_pat	cat_com	licen_lic	finca	cedula	ID_y	bloque	geometry_y
141	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	2422.0	exclusividades_allis	comercial	comercio	n/a	0164006	602760640	2	084	POINT (408919.843 1103457.164)
142	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3363.0	antojitos_caseros	comercial	comercio	n/a	0164005	602310629	2	084	POINT (408919.665 1103476.278)
143	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3058.0	panapager	comercial	comercio	n/a	0164004	3101621626	2	084	POINT (408927.889 1103479.077)
144	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	1157.0	tienda_las_brisas	comercial	comercio	n/a	0234233	3101462428	2	083	POINT (408920.062 1103555.273)
145	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3419.0	farmacia_suyapa	comercial	comercio	n/a	0011340	3101703300	2	083	POINT (408913.177 1103595.027)
146	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3885.0	best_brands	comercial	comercio	n/a	0011436	3102643555	2	083	POINT (408922.758 1103513.489)
147	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3072.0	panaderia_quesada	comercial	comercio	n/a	0032509	3101667382	2	083	POINT (408920.314 1103520.771)
148	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3826.0	panaderia_ppk	comercial	comercio	n/a	0143819	3101151768	2	082	POINT (408845.305 1103495.986)
149	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4631.0	soda_heng	comercial	comercio	n/a	0011339	115600564822	2	083	POINT (408908.340 1103604.953)
150	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4450.0	tienda_el_faro	comercial	comercio	n/a	0201476	800080595	2	082	POINT (408847.971 1103572.753)
151	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	130.0	hotel_sol_y_mar	comercial	servicio	n/a	0136566	202730148	2	082	POINT (408830.540 1103579.207)
152	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4355.0	mundo_barato	comercial	comercio	n/a	0145143	3101734357	2	082	POINT (408883.159 1103544.521)
153	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3736.0	decavisa	comercial	comercio	n/a	0007592	3101220765	2	082	POINT (408885.564 1103532.843)
154	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	1136.0	casa_blanca	comercial	comercio	n/a	0018040	3101353186	2	082	POINT (408817.595 1103537.099)
155	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3806.0	strada	comercial	comercio	n/a	0141406	3101484643	2	082	POINT (408810.200 1103490.845)
156	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	5387.0	m_y_k_boutique	comercial	comercio	cho	0013924	3102775821	2	082	POINT (408811.553 1103513.925)
157	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3227.0	joyeria_salazar	comercial	comercio	n/a	0016055	203800169	2	082	POINT (408864.737 1103585.040)
158	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	5743.0	prestafull	comercial	comercio	n/a	0007612	3101784417	2	082	POINT (408862.937 1103496.074)
159	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	2229.0	moda_belinda	comercial	comercio	n/a	0016051	601640538	2	082	POINT (408876.681 1103594.695)
160	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	5946.0	sala_de_juegos_el_dragon_	comercial	comercio	n/a	0008968	602530154	2	082	POINT (408889.523 1103601.371)
161	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3765.0	zapatto	comercial	comercio	n/a	0011488	3101324076	2	082	POINT (408879.172 1103559.052)
162	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	5831.0	bendimar	comercial	comercio	n/a	0016053	3102816315	2	082	POINT (408870.817 1103589.132)
163	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	2622.0	tienda_continental	comercial	comercio	n/a	0017130	800670990	2	082	POINT (408822.324 1103576.079)
164	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4064.0	la_curacao	comercial	comercio	n/a	0007504	3101074154	2	082	POINT (408810.757 1103561.337)
165	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3836.0	centro_hogar_la_confianza	comercial	comercio	n/a	0175712	3101608244	2	082	POINT (408887.621 1103516.554)
166	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3620.0	calzado_amoretty	comercial	comercio	n/a	0175713	155813512623	2	082	POINT (408887.135 1103523.519)
167	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	5233.0	presto_cash	comercial	comercio	n/a	0015891	3101396483	2	082	POINT (408812.278 1103570.643)
168	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	2980.0	tecnologia_la_confianza	comercial	comercio	n/a	0175711	3101373942	2	082	POINT (408878.624 1103503.751)
169	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4746.0	tienda_maria_cristina	comercial	comercio	n/a	0015887	3101485171	2	082	POINT (408813.769 1103585.550)
170	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4440.0	tienda_angeles	comercial	comercio	sd	0015889	117002350730	2	082	POINT (408808.108 1103586.146)
171	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3804.0	pacific_fashion	comercial	comercio	n/a	0175709	3101477812	2	082	POINT (408884.981 1103502.116)
172	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3213.0	intimidades	comercial	comercio	n/a	0175710	202751246	2	082	POINT (408892.472 1103503.596)
173	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3204.0	novedades_ola	comercial	comercio	n/a	0061798	115600368812	2	082	POINT (408890.755 1103510.404)
174	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3955.0	restaurante_chung_wah	comercial	comercio	b1	0009150	115600165832	2	081	POINT (408892.841 1103473.829)
175	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4577.0	porton_verde	comercial	comercio	n/a	0109428	3101477187	2	081	POINT (408874.648 1103450.614)
176	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3842.0	restaurante_hong_tu	ambas	comercio	e2	0034765	3101626785	2	081	POINT (408827.390 1103467.635)
177	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	5497.0	mini_super_pura_vida_#2	comercial	comercio	n/a	0087841	801100003	2	081	POINT (408862.165 1103472.559)
178	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	2124.0	soda_matilde_(la_ventanit	comercial	comercio	n/a	0094351	600940241	2	081	POINT (408839.575 1103470.199)
179	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3760.0	optica_vision	comercial	comercio	n/a	0036897	3102008400	2	081	POINT (408820.909 1103444.911)
180	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3789.0	elecsport	comercial	servicio	n/a	0145743	3101497721	2	075	POINT (408715.641 1103540.619)
181	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	6042.0	lucky_star_suplidora_de_b	comercial	comercio	n/a	0070535	603120891	2	076	POINT (408764.246 1103464.608)
182	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3768.0	ferreteria_el_campeon	comercial	comercio	n/a	0009473	115600401226	2	076	POINT (408776.100 1103465.469)
183	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3653.0	pops	comercial	comercio	n/a	0009472	3101011086	2	076	POINT (408788.010 1103463.357)
184	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4977.0	pali	ambas	comercio	a	0081699	3102007223	2	075	POINT (408708.678 1103506.086)
185	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4648.0	tienda_kalina	comercial	comercio	n/a	0164500	3102800185	2	076	POINT (408706.784 1103457.437)
186	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	406.0	tienda_cheri	comercial	comercio	n/a	0169884	601020540	2	076	POINT (408751.245 1103461.477)
187	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3727.0	actualidad_sport	comercial	comercio	n/a	0117531	3101206308	2	075	POINT (408782.817 1103503.910)
188	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4508.0	mundo_magico	desocupado	comercio	n/a	0008042	3101244112	2	075	POINT (408782.870 1103545.666)
189	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3852.0	arena_skate_and_surf	comercial	comercio	n/a	0007532	3101662407	2	075	POINT (408783.253 1103511.356)
190	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3837.0	movistar	comercial	servicio	n/a	0007533	3101610198	2	075	POINT (408788.212 1103493.055)
191	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3232.0	tienda_zona_libre_puntare	comercial	comercio	n/a	0108596	3101738723	2	075	POINT (408728.188 1103486.999)
192	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	4378.0	farmacia_puntarenas	comercial	comercio	n/a	0109803	3101571486	2	075	POINT (408706.003 1103487.624)
193	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	5419.0	puntarenas_backpakers_by_	comercial	servicio	n/a	0128600	3101229100	2	074	POINT (408681.516 1103547.242)
194	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	1977.0	tienda_agape	comercial	comercio	n/a	0010880	205350696	2	073	POINT (408827.490 1103627.703)
195	zona comercial	330000.0	u01	2	MULTIPOLYGON (((408784.925 1103619.521, 408785...	3766.0	carnes_de_mi_granja	comercial	comercio	n/a	0007733	3101324494	2	070	POINT (408685.221 1103452.633)

zonas_comercios2.groupby("cat_com")
     
<pandas.core.groupby.generic.DataFrameGroupBy object at 0x7c2d011559f0>

type(zonas_comercios2.groupby("cat_com"))
     
pandas.core.groupby.generic.DataFrameGroupBy

list(zonas_comercios2.groupby("cat_com"))
     
[('comercio',
                         NOMBRE_ZON codigo     VALOR   cat_com  \
  0     sector san lucas beach club    u22  190000.0  comercio   
  1     sector san lucas beach club    u22  190000.0  comercio   
  4     sector san lucas beach club    u22  190000.0  comercio   
  5     sector san lucas beach club    u22  190000.0  comercio   
  13   sector barrio del carmen sur    u21  130000.0  comercio   
  ..                            ...    ...       ...       ...   
  333                    crematorio    u36   40000.0  comercio   
  334                    crematorio    u36   40000.0  comercio   
  335                    crematorio    u36   40000.0  comercio   
  336                    crematorio    u36   40000.0  comercio   
  337                    crematorio    u36   40000.0  comercio   
  
                                              geometry_x  
  0    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  1    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  4    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  5    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  13   MULTIPOLYGON (((408094.849 1103291.980, 408095...  
  ..                                                 ...  
  333  MULTIPOLYGON (((407519.536 1103345.010, 407486...  
  334  MULTIPOLYGON (((407519.536 1103345.010, 407486...  
  335  MULTIPOLYGON (((407519.536 1103345.010, 407486...  
  336  MULTIPOLYGON (((407519.536 1103345.010, 407486...  
  337  MULTIPOLYGON (((407519.536 1103345.010, 407486...  
  
  [243 rows x 5 columns]),
 ('industria',
             NOMBRE_ZON codigo     VALOR    cat_com  \
  132  sector incopesca    u27  190000.0  industria   
  
                                              geometry_x  
  132  MULTIPOLYGON (((408178.295 1103604.005, 408178...  ),
 ('pesca',
             NOMBRE_ZON codigo     VALOR cat_com  \
  136  sector incopesca    u27  190000.0   pesca   
  
                                              geometry_x  
  136  MULTIPOLYGON (((408178.295 1103604.005, 408178...  ),
 ('servicio',
                                  NOMBRE_ZON   codigo     VALOR   cat_com  \
  2              sector san lucas beach club      u22  190000.0  servicio   
  3              sector san lucas beach club      u22  190000.0  servicio   
  6              sector san lucas beach club      u22  190000.0  servicio   
  7              sector san lucas beach club      u22  190000.0  servicio   
  8              sector san lucas beach club      u22  190000.0  servicio   
  ..                                     ...      ...       ...       ...   
  313  barrio el carmen - estadio lito perez      u23  170000.0  servicio   
  314                           las playitas  u03/u04  100000.0  servicio   
  317                           las playitas  u03/u04  100000.0  servicio   
  321                               el cocal      u06   85000.0  servicio   
  328                             crematorio      u36   40000.0  servicio   
  
                                              geometry_x  
  2    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  3    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  6    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  7    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  8    MULTIPOLYGON (((406747.210 1103361.580, 406752...  
  ..                                                 ...  
  313  MULTIPOLYGON (((408216.447 1103366.109, 408217...  
  314  MULTIPOLYGON (((409314.027 1103537.971, 409314...  
  317  MULTIPOLYGON (((409314.027 1103537.971, 409314...  
  321  MULTIPOLYGON (((410404.563 1103607.654, 410393...  
  328  MULTIPOLYGON (((407519.536 1103345.010, 407486...  
  
  [93 rows x 5 columns])]

base = zonas.plot(color='#fffffa', edgecolor='#d2c796', figsize=(20, 20), markersize=10)
patentes.plot(ax=base, marker='o', color='red', edgecolor="black", markersize=7)
     
<Axes: >


base = zonas.plot(column = "VALOR", legend=True, figsize=(20, 20),  legend_kwds={"label": "ZONAS DE VALOR", "orientation": "horizontal"},)
patentes.plot(ax=base, color='white', edgecolor='orange',  markersize=1 )
     
<Axes: >

LOCALES COMERCIALES SEGÚN UBICACIÓN PREDIAL

patentes_catastro = patentes.merge(catastro, on='finca')
patentes_catastro
     
num_pat	nom_com	tipo_pat	cat_com	licen_lic	finca	cedula	ID_x	codigo_x	bloque_x	geometry_x	identifica	plano	bloque_y	predio	ID_y	codigo_y	geometry_y
0	2777.0	hotel_c.r._yacht_club	desocupado	comercio	d2	0021048	3101005849	3	u12	143	POINT (412708.706 1103747.239)	601010021048A0	600112181971	143	003	3	u12	MULTIPOLYGON (((412802.190 1103745.306, 412798...
1	3317.0	soda_ucr	comercial	comercio	n/a	0134536	601001232	3	u08/u09	128	POINT (411148.703 1103802.039)	60101013453600	608501392003	128	006	3	u13/u14	MULTIPOLYGON (((410969.577 1103867.878, 411035...
2	5279.0	ceviches_del_puerto	ambas	comercio	c	0015277	603340776	3	u12	143	POINT (412883.074 1103723.416)	60101001527700	603844391980	143	000	3	u12	MULTIPOLYGON (((412888.011 1103741.692, 412886...
3	5333.0	carvher_pet	comercial	comercio	n/a	0013227	602540562	3	u08/u09	143	POINT (412164.568 1103823.921)	60101001322700	606769031987	143	012	3	u08/u09	MULTIPOLYGON (((412169.649 1103818.019, 412162...
4	3380.0	encuadernacion_el_cocal	comercial	comercio	n/a	0011710	602190453	3	u08/u09	143	POINT (412033.491 1103822.117)	60101001171000	607099181987	143	025	3	u08/u09	MULTIPOLYGON (((412030.072 1103843.004, 412038...
...	...	...	...	...	...	...	...	...	...	...	...	...	...	...	...	...	...	...
400	3818.0	hotel_la_punta	ambas	servicio	e1a	0174660	3101559994	1	u23	001	POINT (406851.985 1103300.416)	60101017466000	601514251993	001	015	1	u23	MULTIPOLYGON (((406857.995 1103317.262, 406858...
401	494.0	bar_restaurante_manglamar	ambas	servicio	c	0180507	601510423	1	u23	002	POINT (406833.861 1103199.381)	60101018050701	614734802011	002	001	1	u23	MULTIPOLYGON (((406840.682 1103195.462, 406828...
402	494.0	bar_restaurante_manglamar	ambas	servicio	c	0180507	601510423	1	u23	002	POINT (406833.861 1103199.381)	60101018050700	614734802011	002	003	1	u23	MULTIPOLYGON (((406836.359 1103221.663, 406824...
403	5752.0	tiki_brunch	ambas	comercio	sd	0176863	601720332	1	u25/u26	001	POINT (406801.429 1103349.859)	60101017686300	607896802002	001	027	1	u25/u26	MULTIPOLYGON (((406814.957 1103319.466, 406812...
404	2947.0	isla_cocos	ambas	comercio	c	0176862	3101283487	1	u25/u26	001	POINT (406789.631 1103344.069)	60101017686200	607872632002	001	026	1	u22	MULTIPOLYGON (((406798.028 1103317.643, 406780...
405 rows × 18 columns


base = catastro.plot(color='#fffffa', edgecolor='#d2c796', figsize=(20, 20), markersize=10)
patentes.plot(ax=base, marker='o', color='red', edgecolor="black", markersize=7)
     
<Axes: >

LOCALES COMERCIALES SEGÚN BARRIOS

barrios_patentes = barrios.merge(patentes, on='ID')
barrios_patentes
     
nombre	ID	geometry_x	num_pat	nom_com	tipo_pat	cat_com	licen_lic	finca	cedula	codigo	bloque	geometry_y
0	barrio_el_carmen	1	MULTIPOLYGON (((408104.200 1103019.393, 407780...	1660.0	aguamarina	ambas	comercio	a	0007844	900250141	u18/u19	047	POINT (408053.908 1103098.806)
1	barrio_el_carmen	1	MULTIPOLYGON (((408104.200 1103019.393, 407780...	4060.0	soda_y_heladeria_y_el_pas	comercial	servicio	n/a	0010824	602590510	u18/u19	047	POINT (408077.399 1103102.180)
2	barrio_el_carmen	1	MULTIPOLYGON (((408104.200 1103019.393, 407780...	6029.0	ocean_marina	comercial	comercio	n/a	0211320	3102845070	u27	043	POINT (407958.709 1103410.080)
3	barrio_el_carmen	1	MULTIPOLYGON (((408104.200 1103019.393, 407780...	5761.0	super_mercado_gallo_pinto	comercial	comercio	sd	0138854	3002344562	u21	046	POINT (408026.418 1103138.917)
4	barrio_el_carmen	1	MULTIPOLYGON (((408104.200 1103019.393, 407780...	5916.0	cabinas_confort	comercial	servicio	n/a	0007574	603750126	u21	046	POINT (408045.462 1103201.356)
...	...	...	...	...	...	...	...	...	...	...	...	...	...
333	el_cocal	3	MULTIPOLYGON (((409547.121 1103338.226, 409517...	3761.0	maes_grill	comercial	comercio	n/a	0182028	3101305784	u15/u16	098	POINT (409710.549 1103411.146)
334	el_cocal	3	MULTIPOLYGON (((409547.121 1103338.226, 409517...	5146.0	sur_quimica_s.a	comercial	comercio	cho	0016228	3101022435	u08/u09	095	POINT (409653.777 1103495.528)
335	el_cocal	3	MULTIPOLYGON (((409547.121 1103338.226, 409517...	5415.0	multiservicios_blanco	comercial	comercio	n/a	0122769	502610924	u05	096	POINT (409622.333 1103457.184)
336	el_cocal	3	MULTIPOLYGON (((409547.121 1103338.226, 409517...	5751.0	bar_el_lucero	ambas	comercio	b1	0229715	604300550	u05	096	POINT (409636.359 1103461.597)
337	el_cocal	3	MULTIPOLYGON (((409547.121 1103338.226, 409517...	5260.0	mariscos_sota	comercial	servicio	n/a	0109589	3101200825	u08/u09	095	POINT (409615.600 1103530.733)
338 rows × 13 columns


from matplotlib import pyplot as plt
import seaborn as sns
barrios_patentes.groupby('nombre').size().plot(kind='barh', color=sns.palettes.mpl_palette('Dark2'),  title='CANTIDAD DE LOCALES COMERCIALES UBICADOS POR BARRIOS DE LA CIUDAD DE PUNTARENAS', x='CANTIDAD DE PATENTES', y='BARRIOS')
plt.gca().spines[['top', 'right',]].set_visible(True)
     


barrios_patentes2 = barrios_patentes[["nombre", "cat_com", "geometry_x"]]
barrios_patentes2
     
nombre	cat_com	geometry_x
0	barrio_el_carmen	comercio	MULTIPOLYGON (((408104.200 1103019.393, 407780...
1	barrio_el_carmen	servicio	MULTIPOLYGON (((408104.200 1103019.393, 407780...
2	barrio_el_carmen	comercio	MULTIPOLYGON (((408104.200 1103019.393, 407780...
3	barrio_el_carmen	comercio	MULTIPOLYGON (((408104.200 1103019.393, 407780...
4	barrio_el_carmen	servicio	MULTIPOLYGON (((408104.200 1103019.393, 407780...
...	...	...	...
333	el_cocal	comercio	MULTIPOLYGON (((409547.121 1103338.226, 409517...
334	el_cocal	comercio	MULTIPOLYGON (((409547.121 1103338.226, 409517...
335	el_cocal	comercio	MULTIPOLYGON (((409547.121 1103338.226, 409517...
336	el_cocal	comercio	MULTIPOLYGON (((409547.121 1103338.226, 409517...
337	el_cocal	servicio	MULTIPOLYGON (((409547.121 1103338.226, 409517...
338 rows × 3 columns


barrios_patentes2.groupby("nombre")
type(barrios_patentes2.groupby("nombre"))
list(barrios_patentes2.groupby("nombre"))
     
[('barrio_el_carmen',
                nombre   cat_com  \
  0   barrio_el_carmen  comercio   
  1   barrio_el_carmen  servicio   
  2   barrio_el_carmen  comercio   
  3   barrio_el_carmen  comercio   
  4   barrio_el_carmen  servicio   
  ..               ...       ...   
  80  barrio_el_carmen  servicio   
  81  barrio_el_carmen  servicio   
  82  barrio_el_carmen  servicio   
  83  barrio_el_carmen  comercio   
  84  barrio_el_carmen  comercio   
  
                                             geometry_x  
  0   MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  1   MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  2   MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  3   MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  4   MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  ..                                                ...  
  80  MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  81  MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  82  MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  83  MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  84  MULTIPOLYGON (((408104.200 1103019.393, 407780...  
  
  [85 rows x 3 columns]),
 ('el_cocal',
         nombre   cat_com                                         geometry_x
  289  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  290  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  291  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  292  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  293  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  294  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  295  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  296  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  297  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  298  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  299  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  300  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  301  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  302  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  303  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  304  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  305  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  306  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  307  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  308  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  309  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  310  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  311  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  312  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  313  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  314  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  315  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  316  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  317  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  318  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  319  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  320  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  321  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  322  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  323  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  324  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  325  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  326  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  327  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  328  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  329  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  330  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  331  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  332  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  333  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  334  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  335  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  336  el_cocal  comercio  MULTIPOLYGON (((409547.121 1103338.226, 409517...
  337  el_cocal  servicio  MULTIPOLYGON (((409547.121 1103338.226, 409517...),
 ('puntarenas_centro',
                  nombre   cat_com  \
  85   puntarenas_centro  comercio   
  86   puntarenas_centro  comercio   
  87   puntarenas_centro  comercio   
  88   puntarenas_centro  servicio   
  89   puntarenas_centro  servicio   
  ..                 ...       ...   
  284  puntarenas_centro  servicio   
  285  puntarenas_centro  servicio   
  286  puntarenas_centro  servicio   
  287  puntarenas_centro  servicio   
  288  puntarenas_centro  servicio   
  
                                              geometry_x  
  85   MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  86   MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  87   MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  88   MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  89   MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  ..                                                 ...  
  284  MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  285  MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  286  MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  287  MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  288  MULTIPOLYGON (((408104.200 1103019.393, 408040...  
  
  [204 rows x 3 columns])]

base = patentes.plot(color='red', edgecolor='#450000', figsize=(20, 20), markersize=5)
barrios.plot(ax=base, marker='o', color='none', edgecolor="black")
     
<Axes: >


base = zonas.plot(column="VALOR", legend = "true", legend_kwds={"label": "VALOR DEL METRO CUADRADO", "orientation": "horizontal"}, figsize=(20, 20))
patentes.plot(ax=base, marker='o', color='red', edgecolor='#450000', markersize=5, )
     
<Axes: >
