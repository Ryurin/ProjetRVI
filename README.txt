
Tutoriel d'utilisation de la scène de projet Unity RVI


Scripts pour votre implémentation :

    - Agent.cs        : 
        Classe abstraite pour l'agent qui sera controlé par la méthode de navigation.

    - AgentExample.cs : 
        Demo d'implémentation de Agent.cs.
        Inspirez vous-en et lisez les commentaires pour associer le comportement que vous désirez dans chaque méthode.
        


   COMMENT APPLIQUER VOTRE SCRIPT :

      L'objet Unity qui doit contenir votre script est "Moving Soldier/soldier"
      Drag 'n' drop votre script à la place de "AgentExample"

      (ne vous occupez pas de "NavigationFPS" en dessous, c'est un script de debug qui doit être DÉSACTIVÉ.)
      








A voir pour compréhension si nécessaire :

    - Door.cs       : 
        L'objet porte à ouvrir. Nécessite deux instances de Key.cs (rouge et verte)
        S'ouvre quand observée et à proximité.

    - Key.cs        : 
        L'objet clés à récupérer.
        Deux exemplaires dans la salle principale.
        Peut être récupérée en marchant dessus ou en la regardant en se situant assez près.

    - CheckPoint.cs : 
        Le contrôle des flags de récupération des clés, d'ouverture d'une porte et du passage à un nouveau tour.

    - FileDialog.cs :
        L'interface de discussion avec le système de fichiers.
        Crée un dossier pour sauvegarder les résultats :

        |Projet Unity
          |Results
            |test.cvs
            |times.csv
            

        Permet de sauvegarder un temps accompli selon le mode de jeu :
          - si mode Free Roaming   (Touche A à n'importe quel  moment) : 
               Sauvegarde chaque tour d'essai (même incomplet) dans le fichier "Results/test.csv"

          - si mode Actual Attempt (Touche R à n'importe quel  moment) : 
               Sauvegarde chaque essai réel dans "Results/times.csv" UNIQUEMENT SI LES TROIS TOURS SONT TERMINÉS


     - Soldier.cs
         classe de Debug. Inutile.


  