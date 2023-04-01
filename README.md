# libft_42

**Libft** est un projet de l'école 42 qui consiste à recoder un certain nombre de fonctions de la bibliothèque standard C ainsi que d'autres fonctions très utiles pour mes futurs projets. Le but est de me familiariser avec la programmation en C et de comprendre le fonctionnement interne de ces fonctions.

Le projet se compose d'un fichier source **"libft.h"** qui contient les prototypes de toutes les fonctions. Le reste des fonctions sont réparties en différents fichiers sources.

Fonctions disponibles

* **ft_memset:** remplit les n premiers octets de la zone mémoire pointée par s avec l'octet c.

* **ft_bzero:** met à zéro les n premiers octets de la zone pointée par s.

* **ft_memcpy:** copie n octets depuis la zone mémoire src vers la zone mémoire dest.

* **ft_memccpy:** copie au maximum n octets depuis la zone mémoire src vers la zone mémoire dest, s'arrête dès qu'elle rencontre l'octet c.

* **ft_memmove:** copie n octets depuis la zone mémoire src vers la zone mémoire dest. Les deux zones peuvent se chevaucher.

* **ft_memchr:** localise la première occurrence de l'octet c dans les n premiers octets de la zone mémoire pointée par s.

* **ft_memcmp:** compare les n premiers octets des zones mémoire s1 et s2.

* **ft_strlen:** calcule la longueur de la chaîne de caractères s.

* **ft_strlcpy:** copie jusqu'à size - 1 caractères depuis la chaîne de caractères src vers dst.

* **ft_strlcat:** concatène jusqu'à size - 1 caractères de la chaîne de caractères src à la chaîne de caractères dst, et ajoute toujours un caractère nul final.

* **ft_strchr:** recherche la première occurrence du caractère c (converti en unsigned char) dans la chaîne de caractères s.

* **ft_strrchr:** recherche la dernière occurrence du caractère c (converti en unsigned char) dans la chaîne de caractères s.

* **ft_strncmp:** compare les n premiers caractères de la chaîne s1 et s2.

* **ft_atoi:** convertit la chaîne de caractères str en entier.

* **ft_isalpha:** vérifie si le caractère est alphabétique.

* **ft_isdigit:** vérifie si le caractère est un chiffre décimal.

* **ft_isalnum:** vérifie si le caractère est alphabétique ou numérique.

* **ft_isascii:** vérifie si le caractère est un code ASCII.

* **ft_isprint:** vérifie si le caractère est imprimable.

* **ft_toupper:** convertit le caractère en majuscule s'il est alphabétique.

* **ft_tolower:** convertit le caractère en minuscule s'il est alphabétique.

* **ft_calloc:** alloue de la mémoire pour un tableau de nmemb éléments de size octets chacun, initialise la mémoire allouée avec des zéros.

* **ft_strdup:** duplique la chaîne de caractères s.

# Utilisation de la bibliothèque

Pour utiliser la bibliothèque, il suffit de compiler les fichiers source avec le Makefile fourni en tapant la commande make. Cela produira une librairie nommée libft.a que vous pouvez ensuite inclure dans votre projet.

Pour inclure la bibliothèque dans votre projet, vous devez ajouter l'option -L suivie du chemin du dossier contenant la bibliothèque et l'option -lft lors de la compilation de votre programme. Par exemple :

`gcc mon_programme.c -L./libft -lft -o mon_programme<sup>`

Il est également possible d'inclure les fichiers source directement dans votre projet, mais cela peut prendre plus de temps pour la compilation. Si vous choisissez cette option, vous devez inclure le fichier libft.h dans vos fichiers source avec la directive `#include "libft.h"`.
