# Transcription d'un manuscrit avec eScriptorium

![eScriptorium](https://upload.wikimedia.org/wikipedia/commons/thumb/2/26/Logo_escriptorium.png/250px-Logo_escriptorium.png)

## Introduction

### Présentation

Ce dépôt est dédié à la validation du séminaire [Bibliothèques numériques, I. Gestion de projet (conception, partage, archivage)](https://pgc.unige.ch/main/teachings/details/2025-32M7128?year=2025&fac=default-value).

Pour ce projet nous avons utilisé [**eScriptorium**](https://fondue.unige.ch/) pour transcrire 12 pages d'un cahier manuscrit qui en compte 250 environ.

Le document choisi s'intitule : _Procès - Verbal de la commission Bel-Air - Commencé le 9 Juillet 1907. Terminé le 9 Mai 1916._

Et nous avons transcrit les pages 183 à 194.

Le but du projet est d'entraîner un modèle à reconnaître les caractères manuscrits puis de pouvoir être en mesure de transcrire automatiquement le reste du ou des documents.

### Méthodologie

Dans un premier temps, nous avons importé nos documents dans eScriptorium puis nous avons délimité des zones pour chacune des pages. Ces zones permettent de structurer l'image avec par exemple une zone dédiée au titre, une autre pour la marge, le corps du texte, etc.

Dans un second temps, nous avons segmenté chacune des lignes des pages de notre corpus. Cela permet au modèle de repérer aisément les lignes du texte. Ces segments sont intégrés dans une zone pour une meilleure précision. Nous avons d'abord testé si le modèle était capable de procéder à la segmentation par lui-même mais cela s'est avéré peu fiable : seules trois pages étaient bien segmentées, les autres n'avaient pas été bien réalisées. 
Une autre étape qui a suivi la segmentation, a été la numérotation des lignes. En effet, le modèle a eu tendance à d'abord numéroter les lignes du corps du texte puis dans un second temps, les lignes dans les marges. Or, cette zone a été utilisée par les différents secrétaires comme endroit où a été noté les sujets abordés dans les paragraphes annexes. Nous avons donc dû numéroter à la main les segments des pages dans un ordre logique de lecture.

Par la suite, nous avons lancé le modèle FoNDUE-GD_v2_fr. Ce dernier a transcrit complètement 8 pages puis n'a transcrit qu'une partie des dernières pages. Sa transcription était totalement erronée même s'il a été étonnament précis avec les noms propres.

Enfin, nous avons transcrit dans la couche "manual" de eScriptorium les pages du cahier. La transcription induit forcément à des choix et des décisions pour maintenir une cohérence tout en tentant d'être au plus proche du texte d'origine, nous avons rédigé en même temps un document sur notre travail. Nous tentons de revenir avec précision sur nos hésitations, choix et interprétations lors de ce travail de transcription.

Enfin, le dépôt Github et sa Page (site internet) ont été créés afin de présenter notre travail.

## Transcriptions et les Commentaires.

Les images d'orgines du manuscrit se trouvent [ICI](https://github.com/mroylem/margaronr.github.io/tree/main/images_compl%C3%A8tes).

Pour les transcriptions, le dossier est accessible [LA](https://github.com/mroylem/margaronr.github.io/tree/main/transcriptions). 
Nous avons extrait les pages au trois formats possibles depuis eScriptorium : [XML](https://github.com/mroylem/margaronr.github.io/tree/main/transcriptions/transcriptions_XML); [TXT](https://github.com/mroylem/margaronr.github.io/tree/main/transcriptions/transcriptions_TXT) ; [ALTO](https://github.com/mroylem/margaronr.github.io/tree/main/transcriptions/transcriptions_ALTO).

Les commentaires sur la transcription sont consultables [ICI](https://github.com/mroylem/margaronr.github.io/blob/main/Commentaires%20pour%20la%20transcription_Romain%20Margaron.md)



## Equipe

**Étudiant** [Romain Margaron](https://ch.linkedin.com/in/romain-margaron-1412b6140)

**Master** [Patrimoine régional et Humanités numériques](https://www.unine.ch/formation/patrimoine-regional-et-humanites-numeriques)
[Université de Neuchâtel](https://www.unine.ch/)

**Professeur**
[Dr.Simon Gabay](https://www.unige.ch/lettres/humanites-numeriques/equipe/collaborateurs/simon-gabay)
[Professeur à l'Université de Genève](https://www.unige.ch/)
