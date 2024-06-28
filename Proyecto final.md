## Análisis Filogenético de la Foca de Weddell
**Camila Yánez**

**28 Junio 2024**

La foca de Weddell (*Leptonychotes weddellii*) es una de las especies de mamíferos marinos más emblemáticas de la Antártida. Conocida por su notable adaptación a las condiciones extremas del hielo marino y su capacidad para sumergirse a grandes profundidades, esta especie representa un componente crucial del ecosistema antártico. 

### Objetivo
Al realizar una filogenia de la foca de Weddell y otras especies de focas antárticas, podemos identificar las conexiones evolutivas entre ellas. Este análisis nos permite entender cómo se agrupan y divergen estas especies dentro de su linaje evolutivo, revelando las relaciones que han dado forma a su desarrollo a lo largo del tiempo.

![](https://polarjournal.ch/wp-content/uploads/2020/11/Weddellrobbe.jpg)  
Este proyecto se centra en la construcción de una filogenia de varias especies de mamíferos, utilizando el gen **CYB561 (cytochrome b561)**. Este gen es parte de la familia de los citocromos, proteínas fundamentales que juegan un papel crucial en la cadena de transporte de electrones, una parte esencial de la respiración celular. 

### Metodología

1. Obtención de secuencias

  Se seleccionaron y descargaron secuencias del gen **CYB561** de las siguientes especies, empleando la base de datos de genes de [NCBI](https://www.ncbi.nlm.nih.gov/gene/):
  ***Enhydra lutris kenyoni*** (Nutria marina), ***Lontra canadensis*** (Nutria de río norteamericana), ***Lutra lutra*** (Nutria europea), ***Eumetopias jubatus*** (León marino de Steller), ***Zalophus californianus*** (León marino de California), Neomonachus schauinslandi (Foca monje de Hawái), ***Halichoerus grypus*** (Foca gris), ***Leptonychotes weddellii*** (Foca de Weddell), ***Mirounga leonina*** (Elefante marino del sur) ***Mirounga angustirostris*** (Elefante marino del norte), ***Phoca vitulina*** (Foca común), ***Ursus maritimus*** (Oso polar), ***Ursus americanus*** (Oso negro), ***Ursus arctos*** (Oso pardo).

2. Edición con [Sublime Text](https://www.sublimetext.com):
	
	Las secuencias fueron editadas para conservar únicamente los nombres de las espeies
  
```
Ambos archivos en formato FASTA se encuentran en la carpeta data.
```

3. Alineamiento de secuencias
  
  Las secuencias editadas fueron alineadas utilizando la herramienta [MAFFT](https://mafft.cbrc.jp/alignment/software/) desde la terminal Git Bash.

```
Los comandos utilizados para este alineamiento se encuentran en la carpeta scripts. El resultado se guardó en la carpeta results.
```

4. Construcción de la Filogenia
   
   Las secuencias alineadas fueron analizadas con [IQ-TREE](http://www.iqtree.org), una herramienta de análisis filogenético que permite la inferencia de árboles filogenéticos mediante métodos de máxima verosimilitud y Bayesianos.
   
5. Visualización de la Filogenia
   Los datos alineados y analizados fueron ingresador en [FigTree](http://tree.bio.ed.ac.uk/software/figtree/) para la generación y visualización del árbol filogenético resultante

```    
En la filogenia destacan tres grupos principales de mamíferos 

Pinnípedos (morado)
Focas Verdaderas (Phocidae), se agrupan en un clado bien definido.
Leones Marinos (Otariidae), forman otro grupo distintivo.

- Mustélidos (rosado)

Las nutrias forman un grupo separado, mostrando sus propias adaptaciones evolutivas a ambientes semiacuáticos.

- Úrsidos (verde)

El oso americano se utilizó como grupo externo en este análisis, encontrándose fuera del clado de los pinnípedos y mustélidos, proporcionando un punto de referencia evolutivo que ayuda a enraizar el árbol y a interpretar las relaciones entre los grupos de mamíferos marinos.
```

![](/Users/camilayanez/Desktop/Pinnipedos/results/Filogenia.jpg?raw=true "Filogenia")



Más sobre los hábitos de la Foca de Weddell:
  
<iframe src="https://www.youtube.com/embed/M5E8gulPWh4?si=ojGBl82rYPjOJsh6"data-external= "1" width="560" height="315"> </iframe> 