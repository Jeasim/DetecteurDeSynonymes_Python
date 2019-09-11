/*********************************************
*					     *
* 	   Projet Oracle - Partie 3 	     *
*	      Jean-Simon Bondaz	     	     *
*	     Jo� Bourgeois-Paquin	     *
*		  Claudia Roy		     *
*					     *
/*********************************************

==============================================
	     3 MODES D'UTILISATION
==============================================
Le pr�sent projet se d�cline en 3 utilisations:

*****************Entrainement*****************
Exemple:

"-e"
	Active le mode entrainement

"-t [taille]"
	D�finit la taille de la fen�tre de lecture

"--enc [encodage]" 
	Encodage de la ressource

"--chemin [chemin] [chemin] ..."
	Chemin relatif/absolu des fichiers sur 
	lesquels s'entrainer.

EXEMPLE : 
Y:\Cooccurrences\src> mainBD.py -e -t 5 --enc utf-8 --chemin textes\GerminalUTF8.txt

******************Recherche*******************

"-r"
	Active le mode recherche

"-t [taille]"
	Taille de la fen�tre voulue

EXEMPLE :
Y: \Cooccurrences\src>mainBD.py -r -t 5 


******************Clustering******************

"-c"
	Active le mode de clustering

"-t [taille]"
	Taille de la fen�tre pour les mots � analyser

"-n [nombre]"
	Nombre de mots et leur distance du centro�des
	� afficher � la fin de l'algorithme.

"--nc [nombre]"
	Nombre de centro�des � g�n�rer al�atoirement

==OPTIONNELS==
"-v"
	Active l'analyse verbale (montre seulement les verbes)
	CETTE OPTION N'AFFICHERA QUE LES VERBES � LA FIN
	DE L'AFFICHAGE (ou ce qui a la m�me graphie qu'un verbe)
 
EXEMPLE:
Y: \Cooccurrences\src>main.py -c -t 10 -n 10 --nc 25 > test\25c10t10a.txt