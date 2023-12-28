Application : Système de Gestion E-Bus

Ce programme implémente un système de gestion E-Bus, permettant aux utilisateurs de gérer et d'interagir avec des informations concernant les passagers, les bus et les réservations. Voici une description détaillée du projet et du rôle des différentes fonctions implémentées dans le code :

Définition des Structures :
Voyageur : Représente un passager avec un identifiant, un prénom (Nom), un nom de famille (Prenom) et un pointeur vers le passager suivant.
Bus : Représente un bus avec un numéro, une destination et une capacité maximale.
Reservation : Contient des détails sur une réservation, y compris un numéro de réservation, un ID de passager, un numéro de bus et un pointeur vers la réservation suivante.
ListeVoyageurs : Gère une liste de passagers, avec un pointeur vers le premier passager et le nombre total de passagers.
ListeReservations : Gère une liste de réservations, avec un pointeur vers la première réservation et le nombre total de réservations.
Fonctions :

creerVoyageur : Crée un nouveau passager avec l'identifiant, le prénom et le nom fournis.

ajouterVoyageursStockes :Lit les détails des passagers à partir d'un fichier (detailsVoyageur.txt) et les ajoute à la liste des passagers.

creercomptevoyageur : Crée un nouveau compte passager en demandant à l'utilisateur de fournir des détails, puis l'ajoute à la liste des passagers. Les détails sont également ajoutés au fichier.

afficherdetailsvoyageurs :Affiche les détails de tous les passagers de la liste.

libererListeVoyageurs :Libère la mémoire allouée pour la liste des passagers.
afficherbus :Lit les détails des bus à partir d'un fichier (detailsBus.txt) et les affiche.

creerReservation :Crée une nouvelle réservation avec les détails fournis.
ajouterReservationsStockees :Lit les détails des réservations à partir d'un fichier (detailsReservation.txt) et les ajoute à la liste des réservations.

estValide :Vérifie si un numéro de bus est valide (entre 1 et 20).

Ajoutnouvellereservation :Ajoute une nouvelle réservation à la liste et ajoute ses détails au fichier.

afficherdetailsreservation :Affiche les détails d'une réservation spécifique.

modifierDetailsReservation :Modifie les détails d'une réservation spécifique et met à jour le fichier.

afficherReservationsVoyageur :Affiche toutes les réservations effectuées par un passager spécifique.

libererListeReservations :Libère la mémoire allouée pour la liste des réservations.

main :
L'interface principale basée sur un menu permet aux utilisateurs d'interagir avec l'application. Les options incluent la création d'un nouveau compte passager, l'affichage des détails des passagers, l'affichage des détails des bus, la création d'une nouvelle réservation, l'affichage des détails d'une réservation, l'affichage des réservations d'un passager spécifique, la modification des détails d'une réservation et la sortie de l'application.
Utilisation :
Pour utiliser le système, les utilisateurs peuvent suivre les invites du menu, qui les guident dans la création de comptes passagers, la gestion des réservations et la consultation des détails. Le programme lit et écrit des informations dans des fichiers externes pour persister les données entre les exécutions.
