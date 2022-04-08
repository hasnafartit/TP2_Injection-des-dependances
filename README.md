# TP2_Injection-des-dependances

dans cette partie on a fait l'injection des dependances en utulisant Spring framework.
Tout d'abord on a crée des insterfaces et des implémentations de ces interfaces.

puis on a commencer par la version XML et on a créé le fichier de configaration(fichier XML).
![image](https://user-images.githubusercontent.com/84719124/162441273-34fd4315-f833-45a3-b1a4-246e646c7b8a.png)

voici l'ecécution du code:

![image](https://user-images.githubusercontent.com/84719124/162442352-831d4259-85cf-4214-a87e-73fac76e913c.png)



si on remplace la classe "dao.DaoImpl" par la classe "ext.DaoImplVWS" dans le fichier de configaration:

![image](https://user-images.githubusercontent.com/84719124/162442433-004ffa58-d13a-4544-a5d8-62fc82276186.png)



Après on a passé à la version Annotation:
  On a utilisé la notion Component qui permet d'instancier une classe et la notion Autowired qui fait l'injection des dependances
  ![image](https://user-images.githubusercontent.com/84719124/162448373-3cab8a9c-b3d9-4978-b62a-f670044156f8.png)
  
  si on a plusieurs implementations d'une interface on peut trouver des probleme lors de l'utilisation de Autowired c'est pourquoi on ajoute la notion Qualifier  qui prmmet d'injecter l'istance qu'on veut . voici des exemple:
  
  ici on a injecté l'istance dao
  ![image](https://user-images.githubusercontent.com/84719124/162451238-719852c1-a878-4e71-98d4-1dea0b2d341c.png)

et ici on a injecter l'instance dao2
![image](https://user-images.githubusercontent.com/84719124/162451416-754180d3-e108-49aa-bef7-512ffa145046.png)


Puis on a fait l'injection par constructeur :

![image](https://user-images.githubusercontent.com/84719124/162450053-9ea4c7af-3c44-412a-81cf-fd17a8e779c2.png)

  
  
  






















Puis on a utilisé cmd pour exécuter quelques commandes de maven

pour compiler l'application : mvn compiler

![image](https://user-images.githubusercontent.com/84719124/162442913-d8bdb027-88c7-4c03-b0df-660320742313.png)


pour executer les test unitaire : mvm test

![image](https://user-images.githubusercontent.com/84719124/162443231-ffc29f92-c655-422d-813f-7f0deb0f0d36.png)


pour compiler, tester et genere les packages : mvn package

![image](https://user-images.githubusercontent.com/84719124/162443524-13acd28d-3f56-4c4d-9ab8-492d20e47706.png)


pour compiler, tester, genere les packages et l'envoyer vers vers repository maven : mvn install

![image](https://user-images.githubusercontent.com/84719124/162443871-f0f783e5-770b-4aec-a6ee-800dcf4b6350.png)


On peut n'est pas utilisé ces commande dans le cmd car elles existent dans l'IDE
![image](https://user-images.githubusercontent.com/84719124/162444072-c870a7e0-42ad-4a1b-9e3d-1d3f8a171b1e.png)




