MY BUDGET — Installation et utilisation

INSTALLER L'APPLICATION
1. Décompressez my-budget.zip.
2. Téléversez TOUT le contenu du dossier my_budget_app à la racine de votre dépôt GitHub (branche publiée par GitHub Pages).
   Important : téléversez tous les fichiers du ZIP à la racine du dépôt. Les polices et les icônes sont des fichiers séparés à conserver tels quels.
3. Activez GitHub Pages si ce n'est pas déjà fait et attendez la publication du site en HTTPS.
4. Sur Android : ouvrez le lien publié dans Chrome, appuyez sur « Installer » dans My Budget ou choisissez « Installer l'application » / « Ajouter à l'écran d'accueil » dans le menu du navigateur.
5. Sur iPhone/iPad : ouvrez le lien dans Safari, appuyez sur Partager, puis « Sur l'écran d'accueil » et « Ajouter ».

L'application est une PWA installable : elle s'ouvre dans sa propre fenêtre, avec son icône, comme une application classique. Elle ne nécessite pas le Play Store.

DONNÉES ET CONNEXION
- Aucune base de données en ligne, aucun compte et aucune synchronisation distante.
- Les données financières sont enregistrées localement sur l'appareil, dans le stockage du navigateur de l'application.
- Après le premier chargement en ligne, les fichiers de l'application sont mis en cache et l'application peut s'ouvrir hors connexion.
- Les données ne sont pas partagées entre plusieurs téléphones.
- Attention : effacer les données du navigateur ou désinstaller l'application peut supprimer les données locales. Faites régulièrement une sauvegarde depuis Paramètres > Sauvegarde des données > Exporter la sauvegarde, et conservez le fichier JSON ailleurs (par exemple dans un espace de fichiers personnel).

FICHES PDF
- Chaque fiche mensuelle propose « Télécharger la fiche PDF » : le fichier est généré directement par l'application, sans fenêtre d'impression et sans envoyer les données sur Internet.
- Le bilan annuel propose également « Télécharger le bilan PDF ».
- Les PDF sont générés sur l'appareil.

POLICES ET CONFIDENTIALITÉ
- Les polices Lato et Accanthis sont fournies avec les fichiers de l’application et mises en cache pour fonctionner hors connexion.
- Aucun service externe n'est utilisé pour générer les fiches PDF.

RAPPELS
- Les rappels de fin de mois, de début de mois et de bilan annuel sont affichés lorsque l'application est ouverte.
- Les notifications automatiques garanties lorsque l'application est complètement fermée nécessiteraient un service push externe ; elles ne sont donc pas promises ici.

COMPTABILITÉ
- Les dépenses fixes configurées sont provisionnées et déduites automatiquement du solde du mois. Ne les saisissez pas une seconde fois dans Mouvements, qui sert aux dépenses ponctuelles.
- Les dépôts d'épargne réduisent le solde disponible ; les retraits l'augmentent. L'épargne est suivie séparément.
- Les données historiques restent modifiables depuis les fiches mensuelles et les mouvements.
