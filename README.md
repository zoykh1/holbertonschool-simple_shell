<img align="center" width="35%" src="https://cdn.prod.website-files.com/64107f65f30b69371e3d6bfa/65c6179aa44b63fa4f31e7ad_Holberton-Logo-Cherry.svg">

# Projet Simple Shell

## Sommaire

<img align="right" width="35%" src="https://cdn-icons-png.flaticon.com/512/1672/1672361.png">

- [Description](#description)
- [Prototype de la fonction](#prototype-de-la-fonction)
- [Fonctionnalités](#fonctionnalités)
- [Compilation](#compilation)
- [Exigences](#exigences)
- [Exemples](#exemples)
- [Man Page](#man-page)
- [Diagramme de flux](#diagramme-de-flux)
- [Tests et Valgrind](#tests-et-valgrind)
- [Auteurs](#auteurs)
- [Notes](#notes)

---

## Description
Ce projet consiste à implémenter un interpréteur de commandes simple, écrit en C, qui reproduit certaines fonctionnalités de `/bin/sh`. Il peut fonctionner à la fois en mode interactif et non interactif.

---

## Prototype de la fonction
```c
int main(int argc, char **argv);

- Exécution de commandes basiques.
- Gestion des erreurs (affichage des messages d'erreur personnalisés).
- Gestion des processus via `fork`, `execve`, et `wait`.
- Utilisation de la variable `PATH` pour localiser les binaires.
- Prise en charge des signaux et gestion du EOF (`Ctrl+D`).

 ```gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh

- **Ubuntu 20.04 LTS**
- **GCC**
- **Git**

$ ./hsh
($) ls
main.c shell.c hsh
($) pwd
/home/user/simple_shell
($) exit







