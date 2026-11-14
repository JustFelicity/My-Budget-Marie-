MY BUDGET — VERSION 17

Application de budget personnel, installable comme PWA et utilisable hors connexion après le premier chargement.

MISE À JOUR
1. Décompressez l'archive.
2. Remplacez les fichiers à la racine de votre dépôt GitHub Pages par les fichiers de cette archive.
3. Conservez la même adresse GitHub Pages et ne supprimez pas les données du navigateur.
4. Rechargez le site. Si l'ancienne version reste affichée, fermez complètement l'application puis rouvrez-la ; le service worker utilise un nouveau cache.

DONNÉES ET MIGRATION
- Les données restent stockées localement dans le navigateur (localStorage, clé mybudget_v1).
- La migration depuis les versions précédentes conserve le profil, les dépenses fixes, les dépenses mobiles, les salaires et les mouvements d'épargne déjà enregistrés.
- Les dates de salaire et de dépenses sont supprimées conformément au nouveau fonctionnement. La date réelle des remboursements de crédit est conservée et ne peut pas être postérieure à la date du jour.
- Avant toute mise à jour importante, exportez une sauvegarde depuis Paramètres.

FONCTIONNEMENT
- Après l'initialisation, choisissez vous-même le mois de référence. Les mois proposés vont de janvier 2020 au mois réel autorisé par le calendrier ; le mois suivant n'apparaît que pendant la dernière semaine du mois réel.
- Tous les onglets suivent le mois consulté. Le bouton de retour ramène au mois de référence.
- Les mois clôturés restent modifiables via « Modifier ce mois ». Les soldes concernés sont recalculés.
- Les dépenses fixes intégrées et personnalisées sont gérées dans Paramètres ; chaque mois conserve ses propres montants. Les dépenses ponctuelles sont appelées « Dépenses mobiles ».
- Lors de l’ajout d’une entrée (prime, cadeau, commission, etc.) à l’accueil, une rubrique dépliable permet, facultativement, d’affecter immédiatement une somme à l’épargne. Si elle reste vide, l’entrée reste disponible dans l’onglet Épargne : vous pouvez alors sélectionner cette entrée et choisir le montant à mettre de côté. Une entrée déjà partiellement affectée reste proposée tant qu’il lui reste un montant disponible ; le montant total affecté peut être modifié ou complété depuis l’accueil ou l’onglet Épargne. Le salaire est également proposé une seule fois dans l’onglet Épargne tant qu’aucune contribution salariale n’a été enregistrée pour le mois. Dès qu’elle est enregistrée, il disparaît des nouvelles possibilités de versement ; son montant affecté reste modifiable depuis la liste des contributions. Chaque affectation diminue le solde disponible du mois et augmente le cumul d’épargne. Les contributions et dépôts sont suivis par mois et par provenance ; les retraits et remboursements utilisent les contributions les plus anciennes en premier.
- Les crédits restent visibles de leur mois de création jusqu'au mois de leur remboursement complet. Les remboursements peuvent provenir de l'épargne cumulée ou du solde d'un mois déterminé. Un remboursement est rattaché au mois consulté, tandis que sa date réelle est conservée séparément.
- Les fiches mensuelles et bilans annuels PDF sont générés localement.

PROTECTION
- Le PIN ou mot de passe est facultatif, proposé pendant l'initialisation et modifiable/supprimable dans Paramètres.
- Le secret est stocké sous forme de dérivé PBKDF2 salé dans le stockage local. C'est un verrou d'accès local, pas un chiffrement complet des données.

VERSION 17
- Les cartes de solde de l'Accueil et de l'Épargne sont dépliables : la composition des entrées et la provenance de l'épargne apparaissent à la demande.
- Ajout des palettes sombres Noir & or et Nuit boréale.


Version 14 : huit palettes (dont les versions sombres Rose, Bleu et Sauge), contrastes renforcés, soldes dépliables avec commande discrète en haut à droite, boutons Salaire et Entrée côte à côte, rubrique Apparence repliable et réorganisation des dépenses fixes par glisser-déposer (poignée tactile).


VERSION 17
- L’affectation à l’épargne est facultative lors de l’ajout d’une entrée. Une action dédiée dans Épargne permet d’ajouter de l’argent ultérieurement, en choisissant la provenance et le montant disponible.
- Le sélecteur « Mois consulté » remplace le bouton Rappels dans l’en-tête, avec une largeur réduite ; l’ancien bloc de sélection sous l’en-tête est supprimé.


Version 14 : lors de l’ajout d’une entrée complémentaire, possibilité facultative d’affecter immédiatement une partie à l’épargne via un menu déroulant. Les versements ultérieurs depuis l’onglet Épargne ne proposent que les entrées complémentaires, jamais le salaire.


VERSION 17
- Les affectations à l’épargne des entrées supplémentaires peuvent être modifiées ou complétées depuis l’accueil et l’onglet Épargne.
- À la clôture, le solde positif peut être réparti entre épargne, plusieurs remboursements de crédits et montant laissé disponible.


Version 18 : le bouton « Ajouter à l’épargne » reste visible dans l’onglet Épargne. Il propose le salaire tant qu’aucune contribution salariale n’a été enregistrée pour le mois, ainsi que les nouvelles entrées de l’accueil encore disponibles. Si aucune provenance n’est disponible, le bouton explique les conditions à remplir.
