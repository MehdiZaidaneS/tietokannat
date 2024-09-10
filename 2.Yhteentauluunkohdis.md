Yhteen tauluun kohdistuvien kyselyiden harjoitukset

### Tehtävä 1
SELECT * FROM goal;
![image](https://github.com/user-attachments/assets/fee26568-0f98-4fc5-8bb5-e40f849de26e)


### Tehtävä 2
SELECT name, type FROM airport WHERE iso_country = "FI";
![image](https://github.com/user-attachments/assets/8116f1ec-d259-45b7-8669-f8baa68ae44e)

 ### Tehtävä 3
SELECT name FROM airport WHERE iso_country = "FI" order by name asc;
 ![image](https://github.com/user-attachments/assets/cb53c375-de4e-41c8-816f-dd28a92a8184)


### Tehtävä 4
SELECT name, type FROM airport WHERE iso_country = "FI" ORDER BY type ASC, name ASC;
 ![image](https://github.com/user-attachments/assets/09f60fe1-175c-4aa1-87f8-e4bcea9f735e)

 ### Tehtävä 5
SELECT name FROM country WHERE name LIKE "F%";
 ![image](https://github.com/user-attachments/assets/a5bff022-ae2a-4dda-be79-901ee773d487)

 ### Tehtävä 6
 SELECT name FROM country WHERE name like "%F%";
 ![image](https://github.com/user-attachments/assets/3db1d915-422c-4791-9f87-c64dbd3530c2)

 ### Tehtävä 7
 SELECT location FROM game WHERE screen_name = "Vesa";
 ![image](https://github.com/user-attachments/assets/6dae9b80-a414-4834-8087-795e2df5393c)

### Tehtävä 8
SELECT co2_consumed FROM game WHERE screen_name = "Ilkka";
 ![image](https://github.com/user-attachments/assets/07d36005-039c-4265-bea3-d25dfb8ebcc8)

 ### Tehtävä 9
SELECT co2_budget FROM game WHERE id= "1";
 ![image](https://github.com/user-attachments/assets/88e6793e-b529-4d7f-971c-db1f6915b388)






