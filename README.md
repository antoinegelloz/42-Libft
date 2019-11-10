# libft
Pour ce premier projet à 42, il faut re-coder des fonctions essentielles de la librairie C standard et d'autres utilitaires ajoutées au cours du cursus.
Ces fonctions servent de base pour les projets C suivants car la librairie standard C est interdite.

## Partie 1
### Implémentation de fonctions de la lib C :
* ft_memset
* ft_bzero
* ft_memcpy
* ft_memccpy
* ft_memmove
* ft_memchr
* ft_memcmp
* ft_strlen
* ft_strdup
* ft_strcpy
* ft_strncpy
* ft_strcat
* ft_strncat
* ft_strlcat
* ft_strchr
* ft_strrchr
* ft_strstr
* ft_strnstr
* ft_strcmp
* ft_strncmp
* ft_atoi
* ft_isalpha
* ft_isdigit
* ft_isalnum
* ft_isascii
* ft_isprint
* ft_toupper
* ft_tolower


## Partie 2
#### ft_memalloc
> Alloue (avec malloc(3)) et retourne une zone de mémoire
> “fraiche”. La mémoire allouée est initialisée à 0. Si l’allocation
> échoue, la fonction renvoie NULL.
#### ft_memdel
> Prend en paramètre l’adresse d’un pointeur dont la zone pointée doit être libérée 
> avec free(3), puis le pointeur est mis à NULL.
#### ft_strnew
> Alloue (avec malloc(3)) et retourne une chaîne de caractère
> “fraiche” terminée par un ’\0’. Chaque caractère de la chaîne
> est initialisé à ’\0’. Si l’allocation echoue, la fonction renvoie NULL.
#### ft_strdel
> Prend en paramètre l’adresse d’une chaîne de caractères qui
> doit être libérée avec free(3) et son pointeur mis à NULL.
#### ft_strclr
> Assigne la valeur ’\0’ à tous les caractères de la chaîne passée
> en paramètre.
#### ft_striter
> Applique la fonction f à chaque caractère de la chaîne de
> caractères passée en paramètre. Chaque caractère est passé
> par adresse à la fonction f afin de pouvoir être modifié si
> nécessaire.
#### ft_striteri
> Applique la fonction f à chaque caractère de la chaîne de
> caractères passée en paramètre en précisant son index en premier argument.
> Chaque caractère est passé par adresse à la
> fonction f afin de pouvoir être modifié si nécessaire.
#### ft_strmap
> Applique la fonction f à chaque caractère de la chaîne de caractères
> passée en paramètre pour créer une nouvelle chaîne
> “fraiche” (avec malloc(3)) résultant des applications successives de f.
#### ft_strmapi
> Applique la fonction f à chaque caractère de la chaîne de
> caractères passée en paramètre en précisant son index pour
> créer une nouvelle chaîne “fraiche” (avec malloc(3)) résultant
> des applications successives de f.
#### ft_strequ
> Compare lexicographiquement s1 et s2. Si les deux chaînes
> sont égales, la fonction retourne 1, ou 0 sinon.
#### ft_strnequ
> Compare lexicographiquement s1 et s2 jusqu’à n caractères
> maximum ou bien qu’un ’\0’ ait été rencontré. Si les deux
> chaînes sont égales, la fonction retourne 1, ou 0 sinon.
#### ft_strsub
> Alloue (avec malloc(3)) et retourne la copie “fraiche” d’un
> tronçon de la chaîne de caractères passée en paramètre. Le
> tronçon commence à l’index start et a pour longueur len. Si
> start et len ne désignent pas un tronçon de chaîne valide,
> le comportement est indéterminé. Si l’allocation échoue, la
> fonction renvoie NULL.
#### ft_strjoin
> Alloue (avec malloc(3)) et retourne une chaîne de caractères
> “fraiche” terminée par un ’\0’ résultant de la concaténation
> de s1 et s2. Si l’allocation echoue, la fonction renvoie NULL.
#### ft_strtrim
> Alloue (avec malloc(3)) et retourne une copie de la chaîne
> passée en paramètre sans les espaces blancs au debut et à la
> fin de cette chaîne. On considère comme espaces blancs les
> caractères ’ ’, ’\n’ et ’\t’. Si s ne contient pas d’espaces
> blancs au début ou à la fin, la fonction renvoie une copie de
> s. Si l’allocation echoue, la fonction renvoie NULL.
#### ft_strsplit
> Alloue (avec malloc(3)) et retourne un tableau de chaînes de
> caractères “fraiches” (toutes terminées par un ’\0’, le tableau
> également donc) résultant de la découpe de s selon le caractère
> c. Si l’allocation echoue, la fonction retourne NULL.
#### ft_itoa
> Alloue (avec malloc(3)) et retourne une chaîne de caractères
> “fraiche” terminée par un ’\0’ représentant l’entier n passé
> en paramètre. Les nombres négatifs doivent être gérés.
> Si l’allocation échoue, la fonction renvoie NULL.
#### ft_putchar
> Affiche le caractère c sur la sortie standard.
#### ft_putstr
> Affiche la chaîne s sur la sortie standard.
#### ft_putendl
> Affiche la chaîne s sur la sortie standard suivi d’un ’\n’.
#### ft_putnbr
> Affiche l’entier n sur la sortie standard.
#### ft_putchar_fd
> Ecrit le caractère c sur le descripteur de fichier fd.
#### ft_putstr_fd
> Ecrit la chaîne s sur le descripteur de fichier fd.
#### ft_putendl_fd
> Ecrit la chaîne s sur le descripteur de fichier fd suivi d’un ’\n’.
#### ft_putnbr_fd
> Ecrit l’entier n sur le descripteur de fichier fd.


## Partie Bonus
#### ft_lstnew
> Alloue (avec malloc(3)) et retourne un maillon “frais”. Les
> champs content et content_size du nouveau maillon sont initialisés par
> copie des paramètres de la fonction. Si le paramètre content est nul,
> le champs content est initialisé à NULL et le champs content_size est
> initialisé à 0 quelque soit la valeur du paramètre content_size. Le champ next
> est initialisé à NULL. Si l’allocation échoue, la fonction renvoie NULL.
#### ft_lstdelone
> Prend en paramètre l’adresse d’un pointeur sur un maillon et
> libère la mémoire du contenu de ce maillon avec la fonction
> del passée en paramètre puis libère la mémoire du maillon
> en lui même avec free(3). La mémoire du champ next ne
> doit en aucun cas être libérée. Pour terminer, le pointeur sur
> le maillon maintenant libéré doit être mis à NULL (de manière
> similaire à la fonction ft_memdel de la partie obligatoire).
#### ft_lstdel
> Prend en paramètre l’adresse d’un pointeur sur un maillon et libère la mémoire
> de ce maillon et celle de tous ses successeurs l’un après l’autre avec del et free(3).
> Pour terminer, le pointeur sur le premier maillon maintenant libéré doit être
> mis à NULL (de manière similaire à la fonction ft_memdel de la partie obligatoire).
#### ft_lstadd
> Ajoute l’élément new en tête de la liste.
#### ft_lstiter
> Parcourt la liste lst en appliquant à chaque maillon la fonction f.
#### ft_lstmap
> Parcourt la liste lst en appliquant à chaque maillon la fonction f et crée
> une nouvelle liste “fraiche” avec malloc(3) résultant des applications successives.
> Si une allocation échoue, la fonction renvoie NULL.


## get_next_line
Retourne une ligne lue depuis un file descriptor (gestion de plusieurs file descriptors simultanément).


## ft_printf
Implementation de la fonction printf
* Conversions supportées : CcSspDdiUuOoXxFfp%*
* Ajout de la conversion B/b pour base binaire
* Flags supportés : h,hh,l,ll,L,z,j,#,0,-,+
* Precision et taille minimum de champs supportés
