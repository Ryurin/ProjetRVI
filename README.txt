
Tutoriel d'utilisation de la sc�ne de projet Unity RVI


Scripts pour votre impl�mentation :

    - Agent.cs        : 
        Classe abstraite pour l'agent qui sera control� par la m�thode de navigation.

    - AgentExample.cs : 
        Demo d'impl�mentation de Agent.cs.
        Inspirez vous-en et lisez les commentaires pour associer le comportement que vous d�sirez dans chaque m�thode.
        


   COMMENT APPLIQUER VOTRE SCRIPT :

      L'objet Unity qui doit contenir votre script est "Moving Soldier/soldier"
      Drag 'n' drop votre script � la place de "AgentExample"

      (ne vous occupez pas de "NavigationFPS" en dessous, c'est un script de debug qui doit �tre D�SACTIV�.)
      








A voir pour compr�hension si n�cessaire :

    - Door.cs       : 
        L'objet porte � ouvrir. N�cessite deux instances de Key.cs (rouge et verte)
        S'ouvre quand observ�e et � proximit�.

    - Key.cs        : 
        L'objet cl�s � r�cup�rer.
        Deux exemplaires dans la salle principale.
        Peut �tre r�cup�r�e en marchant dessus ou en la regardant en se situant assez pr�s.

    - CheckPoint.cs : 
        Le contr�le des flags de r�cup�ration des cl�s, d'ouverture d'une porte et du passage � un nouveau tour.

    - FileDialog.cs :
        L'interface de discussion avec le syst�me de fichiers.
        Cr�e un dossier pour sauvegarder les r�sultats :

        |Projet Unity
          |Results
            |test.cvs
            |times.csv
            

        Permet de sauvegarder un temps accompli selon le mode de jeu :
          - si mode Free Roaming   (Touche A � n'importe quel  moment) : 
               Sauvegarde chaque tour d'essai (m�me incomplet) dans le fichier "Results/test.csv"

          - si mode Actual Attempt (Touche R � n'importe quel  moment) : 
               Sauvegarde chaque essai r�el dans "Results/times.csv" UNIQUEMENT SI LES TROIS TOURS SONT TERMIN�S


     - Soldier.cs
         classe de Debug. Inutile.


  