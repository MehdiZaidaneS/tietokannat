Koostetieto kyselyt harjoitukset

### Tehtävä 1:
SELECT max(elevation_ft) FROM airport;

![image](https://github.com/user-attachments/assets/302bfc9b-05d7-480e-a7b4-21f323c0e10e)

### Tehtävä 2:
SELECT continent, count(*) FROM country GROUP BY continent;

![image](https://github.com/user-attachments/assets/47832422-b41a-4f7e-af81-7ebe32d7491c)


### Tehtävä 3:
select screen_name, count(*)
from game, goal_reached
where id = game_id
group by screen_name;

![image](https://github.com/user-attachments/assets/2bf6010a-69cd-4301-b82d-18f2d4c38364)


### Tehtävä 4:
SELECT screen_name FROM game WHERE co2_consumed IN(
SELECT min(co2_consumed) from game);

![image](https://github.com/user-attachments/assets/ee427919-3852-4f2b-b4e7-c50659c87da0)

### Tehtävä 5:

SELECT country.name, count(*) FROM country, airport
WHERE country.iso_country = airport.iso_country
GROUP BY country.name ORDER BY count(*) DESC LIMIT 50;

![image](https://github.com/user-attachments/assets/00f13946-0c3d-42b0-a677-eb7ba33f532f)

### Tehtävä 6:
SELECT country.name FROM country, airport
WHERE airport.iso_country = country.iso_country
GROUP BY country.iso_country
having count(*) >= 1000;

![image](https://github.com/user-attachments/assets/9371996e-b3ce-4c13-8396-3f58e9296508)

### Tehtävä 7:
SELECT name FROM airport
WHERE elevation_ft IN(
SELECT max(elevation_ft) FROM airport);

![image](https://github.com/user-attachments/assets/53104953-bb35-4e4e-9961-524bd0f668bd)


### Tehtävä 8:
SELECT name FROM country
WHERE iso_country IN(
SELECT iso_country FROM airport
WHERE elevation_ft IN(
SELECT max(elevation_ft) FROM airport));

![image](https://github.com/user-attachments/assets/d28365af-86ce-4347-8be9-97ada2b676d6)

### Tehtävä 9:
SELECT count(*) FROM game, goal_reached
WHERE screen_name = "Vesa" AND game.id = goal_reached.game_id;

![image](https://github.com/user-attachments/assets/f5179417-a524-4495-9889-6e87b29d5657)


### Tehtävä 10:
SELECT name FROM airport
WHERE latitude_deg IN(
SELECT min(latitude_deg) FROM airport);

![image](https://github.com/user-attachments/assets/e9a316d2-9344-4383-8d56-879e313b8f56)
