Calendar & Growth Pro — Démarrage rapide
Documentation de la version candidate 2.1.0 ; pas encore publiée.

1. Copiez addons/rpg_time dans le projet. Activez le plugin dans Project > Project Settings > Plugins. Extrayez le projet d’exemple séparément et ouvrez son project.godot ; ne remplacez pas celui de votre jeu.
2. Ouvrez Time & Seasons et choisissez Français dans Language. Le panneau ne change ni la langue de Godot ni celle du jeu.
3. Dans Configuration, choisissez un chemin res:// hors de addons puis enregistrez le profil. Les champs ne prennent effet qu’après Appliquer. Appliquez ou rétablissez avant de changer de section.
4. Dans Calendrier, définissez mois, jours et saisons. Les noms personnalisés restent inchangés. La première période commence à 00:00 ; les suivantes doivent commencer plus tard.
5. Pour la croissance, choisissez un préréglage puis ajustez le rythme. Vous pouvez modifier séparément maturité et étapes. Déplacer le curseur ou changer de préréglage remplace ces modifications. Les valeurs concernent la prochaine scène générée.
6. Enregistrez le profil puis générez l’ensemble voulu. Glissez la scène dans votre monde ou utilisez l’insertion du panneau. Gardez une seule horloge de référence ; n’ajoutez pas un second CanvasModulate à un canevas déjà connecté.
7. L’aperçu teste temps, saisons et événements sans modifier l’horloge du jeu ni les sauvegardes. Les sauts de plus de 10 000 occurrences sont refusés.

Les contrôles réutilisables possèdent interface_language dans l’Inspector. Après un changement en jeu, appelez refresh(). Les titres, noms et messages personnalisés sont à traduire dans votre système de contenu. Laissez le texte du bouton de sommeil vide pour sa légende traduite automatique.

save_file/load_file sauvegardent l’horloge, pas un jeu complet. Conservez les sauvegardes originales lors d’un essai de mise à jour. Modifier le calendrier ou les événements peut nécessiter une migration. Les profils d’atmosphère facultatifs étendent l’éclairage de base ; météo, combat et déplacement des PNJ ne sont pas inclus.


Atmosphère et outils de développement
Dans Éclairage, choisissez puis appliquez un préréglage d’atmosphère. Les interrupteurs conservent les courbes modifiées manuellement. Enregistrez le profil et générez une nouvelle configuration. Dans l’exemple facultatif Lumen Vale, ouvrez Calendrier et faites défiler jusqu’à Atmosphère. Sans atmosphère conserve le rendu initial. L’aperçu et l’interrupteur de brouillard ne modifient pas le profil enregistré ; retirer l’aperçu restaure l’éclairage initial.

Les outils de développement locaux sont inclus uniquement sur sélection explicite lors de la génération. Désactivés par défaut, ils se relient automatiquement à l’horloge lorsqu’ils sont inclus, mais restent désactivés dans l’exécutable de distribution. DEVELOPMENT-BRIDGE.md décrit le contrat local Fableweld ; aucun accès réseau n’est ouvert.
