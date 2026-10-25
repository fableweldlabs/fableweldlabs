# Inventaire et équipement — démarrage rapide

Inventaire et équipement 1.0.0. Godot 4.7.2, Windows x64. Consultez la licence et les mentions des composants incluses.

1. Conservez une copie du projet et des sauvegardes. Copiez
   `addons/fableweld_inventory` dans le jeu. Comparez les versions et préservez
   vos modifications avant tout remplacement. Aucun addon d’horloge ou de PNJ
   n’est nécessaire.
2. Activez Fableweld Inventory & Equipment dans les paramètres du projet,
   section Plugins. Choisissez la langue du dock ; la langue globale du jeu reste inchangée.
3. Créez des objets ou ajoutez les objets de départ. Modifiez-les dans
   l’inspecteur, validez le catalogue et enregistrez un `.tres` hors de `addons`.
   Chargez une destination existante avant de la mettre à jour ; le chargement
   demande confirmation. Gardez les ID d’objets stables.
4. Ouvrez `demo/inventory_quick_start.tscn` dans le projet d’exemple et appuyez
   sur F6. Le sélecteur supérieur coordonne les onglets et panneaux. Équipez la
   lame de départ, affectez une potion au raccourci, séparez une pile et
   transférez des objets vers le coffre.
5. Dans vos scènes, faites pointer `controller_path` des panneaux vers un
   `FWSlotInventoryController`. Les grilles qui échangent des objets doivent
   partager le catalogue et un `transfer_group` non vide. Le jeu fournit les
   effets des objets et les caractéristiques de base.
6. Enregistrez les contrôleurs dans `FWInventorySession.controllers` avec des ID
   de sauvegarde stables et des NodePaths. Reliez
   `FWInventorySavePanel.session_path` à cette session. Choisissez un chemin
   `user://...json` distinct pour chaque emplacement de sauvegarde ou monde.
7. Enregistrez et chargez la session d’inventaire. Elle comprend sacs enregistrés,
   équipement et raccourcis, mais pas le jeu entier. L’ancien exemple perd son
   point de contrôle en mémoire à la fermeture. Préservez tout fichier
   `.fw-writing` existant avant de réessayer une sauvegarde bloquée. Les écritures
   concurrentes ne sont pas prises en charge.
8. Testez les mises à jour sur une copie. Gardez vos catalogues, scènes et
   sauvegardes hors des dossiers fournisseur. Pour retirer l’addon, remplacez les
   références dépendantes, désactivez le plugin puis supprimez son dossier.
   Supprimer des scripts encore référencés casse les scènes.

La langue préserve les ID et le texte personnalisé. La traduction des catégories
et caractéristiques d’exemple s’active avec `translate_example_names`, désactivé
par défaut dans les vues réutilisables. Le texte personnalisé inconnu reste
intact. Aucune relecture par un locuteur natif, compatibilité universelle ou
acceptation finale des paquets exportés n’est revendiquée.
