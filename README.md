#projet-jo

## Conception UML – Mise en œuvre – Jeux Olympiques

### Introduction

On modélise le traitement de données par un diagramme de séquence en UML.
Les données brutes sont en Semicolumn-separated Value (SSV).
Les données finales sont potentiellement en SQL.

Toute la conception est décrite dans le répertoire `/conception/`.

### Modèles de donnée en MERISE

Les modèles sont construits via l’outil Looping.
Les fichiers `/conception/MCD.png` et `/conception/MLD.png` correspondent
respectivement aux modèles conceptuel et physique de donnée.

Un modèle conceptuel de données définit la base de données finales.
Il est minimal en l’absence d’un cahier des charges.

Le modèle physique de données offre un aperçu plus fidèle de ce que peut
être une base en SQL.

### Diagramme de classe en UML

Les diagrammes sont construits via l’outil StarUML.
Les fichiers  respectifs `/conception/ClassDiagram.svg` et
`/conception/SequenceDiagram.png` correspondent aux diagrammes de classe
et de séquence.

On représente les données brutes par une première classe entité
`LegacyAthlete` dans le paquet `dao`.
On convertit ces données selon les classes du paquet `bo`.

### Diagramme de séquence en UML

Enfin on indique un cas d’usage par une séquence d’actions qu’initie un
administrateur `admin`.
