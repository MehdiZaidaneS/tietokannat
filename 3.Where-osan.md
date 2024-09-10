Where-osan liitosehto harjoitukset


### Tehtävä 1:
SELECT country.name as "country name", airport.name as "airport name" 
FROM country, airport
WHERE country.iso_country = airport.iso_country and country.name = "Iceland";

![image](https://github.com/user-attachments/assets/ed5253b5-abdd-46a6-90b8-ce07c1631e1c)

### Tehtävä 2:
SELECT airport.name as "airport name"
FROM airport, country
WHERE airport.iso_country = country.iso_country and country.name = "France" and airport.type = "large_airport";

![image](https://github.com/user-attachments/assets/e9ccf1ec-0d75-4dcd-bf42-a38a9330f982)

### Tehtävä 3:
select country.name as country_name, airport.name as airport_name
from airport, country
where airport.iso_country = country.iso_country and country.continent = "AN";

![image](https://github.com/user-attachments/assets/d696915b-a10d-48ce-8e0a-fb82d2635ea3)

### Tehtävä 4:
select airport.elevation_ft
from airport, game
where game.screen_name = "Heini" and game.location = airport.ident;

![image](https://github.com/user-attachments/assets/6e640362-719f-4bfa-bb2a-80d28c69ab25)


### Tehtävä 5:
select airport.elevation_ft * 0.3048 as elevation_m
from airport, game
where game.screen_name = "Heini" and game.location = airport.ident;

![image](https://github.com/user-attachments/assets/f773926a-ff95-46e1-9006-1835ee8f906c)


### Tehtävä 6:
select airport.name
from airport, game
where game.screen_name = "Ilkka" and game.location = airport.ident;

![image](https://github.com/user-attachments/assets/0866bac8-2df5-486c-b98b-d5b6cb73d601)


### Tehtävä 7:
select country.name
from airport, game, country
where game.screen_name = "Ilkka" and game.location = airport.ident and airport.iso_country = country.iso_country;

![image](https://github.com/user-attachments/assets/02c88e76-6114-45e4-88b6-fc794ccebae1)


### Tehtävä 8:
select goal.name
from goal, goal_reached, game
where game.screen_name = "Heini" and game.id = goal_reached.game_id and goal_reached.goal_id = goal.id;

![image](https://github.com/user-attachments/assets/9e5c4484-ab6b-46df-b8c6-3d03c445ba88)

### Tehtävä 9:
select airport.name
from airport, goal, goal_reached, game
where goal.name = "clouds" and goal.id = goal_reached.goal_id and goal_reached.game_id = game.id and game.screen_name = "Ilkka" and game.location = airport.ident

![image](https://github.com/user-attachments/assets/ad8c1bca-423b-4d36-aff3-975fdfc90e24)


### Tehtävä 10:
select country.name
from country, airport, goal, goal_reached, game
where goal.name = "clouds" and goal.id = goal_reached.goal_id and goal_reached.game_id = game.id and game.screen_name = "Ilkka" and game.location = airport.ident and airport.iso_country = country.iso_country;

![image](https://github.com/user-attachments/assets/91a88de1-6655-41b6-aa5b-568d69f5fa49)

