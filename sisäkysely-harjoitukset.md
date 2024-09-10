Sisäkysely harjoitukset

### Tehtävä 1:
SELECT name FROM country
WHERE iso_country IN(
SELECT iso_country FROM airport WHERE airport.name LIKE 'Satsuma%');

![image](https://github.com/user-attachments/assets/416d5614-e3c2-4a58-910a-773ab7567dd7)

### Tehtävä 2:
SELECT name FROM airport
WHERE iso_country IN(
SELECT iso_country FROM country WHERE country.name = 'Monaco');

![image](https://github.com/user-attachments/assets/fb4174bf-bbf0-4992-b1d4-d1044b53e776)


### Tehtävä 3:
SELECT screen_name FROM game
WHERE id IN(
SELECT game_id FROM goal_reached
WHERE goal_id IN(
SELECT id FROM goal WHERE name = 'CLOUDS'));

![image](https://github.com/user-attachments/assets/b1915ad9-d1cb-439c-96e1-cb666a82a0e6)


### Tehtävä 4:
SELECT name FROM country
WHERE iso_country NOT IN(
SELECT iso_country FROM airport);

![image](https://github.com/user-attachments/assets/73658457-c529-48c0-9b46-5b34243ea9ab)


### Tehtävä 5:
SELECT name FROM goal
WHERE id NOT IN(
SELECT goal_id FROM goal_reached
WHERE game_id IN(
SELECT id FROM game WHERE screen_name = 'Heini'));

![image](https://github.com/user-attachments/assets/82e3675d-2bf3-42ca-9a65-bab536fe3aea)




