FIRST 
generer l'executable 
gcc -Wall essai.c -o essai
g++ -Wall essai.cpp -o essai

genere en assembleur 
gcc -S essai.c
g++ -S essai.cpp

executer 
./essai


SECOND
generer fichier objet (compiler uniquement, sans linker)
gcc -Wall -c essai.c
gcc -Wall -c function.c

Edition des lien 
gcc essai.o mesfonctions.o -o essai

genere en assembleur 
gcc -S essai.c



Les librairies statiques sont intégrée dans l'exécutable de notre programme au moment de l'édition des liens.

Les librairies dynamiques ne sont pas intégrées à notre programme au moment de l'édition des liens mais sont chargées en mémoire et appelées de façon dynamique lors de l'exécution de notre programme

Pour les fichiers librairies, on rencontre les types d'extensions suivants :
.a = statique (GCC Linux)
.so = dynamique (GCC Linux)
.lib = statique (Microsoft Windows)
.dll = dynamique (Microsoft Windows)

