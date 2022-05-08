## Activité pratique : student-management-spring-mvc
L’énoncé de l’activité 
![img.png](img.png)
    1. Les dépendances :
pour construire cette application on a utilisé un ensemble des dépendances suivants  :
![img_1.png](img_1.png)
![img_2.png](img_2.png)
![img_3.png](img_3.png)
![img_4.png](img_4.png)


    2. Le fichier configuration :
![img_5.png](img_5.png)
    3. L’entité Etudiant :
![img_6.png](img_6.png)
    • La table Etudiant dans la base de données :
![img_7.png](img_7.png)
    • Le type énumération : Genre
![img_8.png](img_8.png)


       4. l'interface EtudiantRepository : 
     Cet interface contient des fonction prédéfinie qui permet d’interagir avec la base de donnée (ajout,suppression,modification…).
![img_9.png](img_9.png)       
5. EtudiantController : 
         cette classe représente le contrôleur de l’application qui s’occupe de répondre aux requêtes du client en lui transmettant les vues.
![img_10.png](img_10.png)






    • Les fonctionnalités de l’application :
    • La recherche des étudiants par nom : 
Voici la fonction déclarée dans le contrôleur et qui permet de retourner les étudiants par mot clé en fait il prend le mot clé comme argument et il stocke le résultat dans le modèle:
![img_11.png](img_11.png)
2. La pagination :
voici la partie de code de la fonction index qui est occupée de gérer la pagination.
![img_12.png](img_12.png)
![img_13.png](img_13.png)
Dans l’interface graphique(vue) on affiche dix pages et deux bouton un pour passer à la page suivante et un autre bouton pour la page précédente.
![img_14.png](img_14.png)
3. La suppression des étudiants  :
![img_15.png](img_15.png)


      4. L’ajout d’un étudiant : 
Voici la méthode qui permet d’ajouter un nouveau étudiant :
![img_16.png](img_16.png)
La page html qui contient le formulaire d’ajout :
![img_17.png](img_17.png)
![img_18.png](img_18.png)
![img_19.png](img_19.png)



      5. La modification d’un étudiant : 
      Voici la méthode qui permet de modifier un étudiant :
      
![img_20.png](img_20.png)

![img_21.png](img_21.png)

      6. La page template  : 
      a) nameSpace de thymleaf et de la spring-security  :
![img_22.png](img_22.png)

      b) les librairies utilisés dans la page template  (bootstrap,bootstrap-icons,fontAwsome,bootstrap-bundle) :
![img_23.png](img_23.png)
      c) navBar  :
![img_24.png](img_24.png)
![img_25.png](img_25.png)

      d) footer : 
      ![img_26.png](img_26.png)
![img_27.png](img_27.png)





      7. La sécurité de l’application  : 
Pour sécuriser l’application on a utilisé un système d’authentification qui est basé sur la stratégie userDetails service voici la structure suivi :


![img_28.png](img_28.png)



    • Les entités de la système d’authentification : 
    1. AppUser :
![img_29.png](img_29.png)



    2. AppRole :
![img_30.png](img_30.png)
    • La classe SecurityConfig : 
      Dans cette méthode  on spécifie la stratégie de la sécurité a utiliser dans l’application : 

![img_31.png](img_31.png)










    • Dans cette méthode  on gère les routes de l’application et les droit d’accès  : 

![img_32.png](img_32.png)






      8. Personnalisé l’authentification     : 
                1.  La méthode login :

![img_33.png](img_33.png)








                      2. La page login :


![img_34.png](img_34.png)
![img_35.png](img_35.png)
![img_36.png](img_36.png)
      9. La page error 404     : 
Cette page apparaît  quand une ressource demandée est indisponible :
![img_37.png](img_37.png)
![img_39.png](img_38.png)




      10. La page error 403     : 
Cette page apparaît  quand une ressource demandée n’est pas autorisé :
![img_38.png](img_39.png)
![img_40.png](img_40.png)











Les pages de l’application :
1) La page d’accueil :
Cette page est accessible à tous :

![img_41.png](img_41.png)




    2) La page d’authentification :


![img_42.png](img_42.png)





    3) La page de la recherche :
              


![img_43.png](img_43.png)


    4) La page d’ajout :
       
![img_44.png](img_44.png)





    5) La page de modification :
       


![img_45.png](img_45.png)



