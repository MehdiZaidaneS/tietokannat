Join harjoitukset

### Tehtävä 1:
select country.name as "country name", airport.name as "airport name"
from country inner join airport on airport.iso_country = country.iso_country
where country.name = "Finland" and scheduled_service = "yes";

![image](https://github.com/user-attachments/assets/78116c68-3543-4bde-bbc7-8602e5023dd6)


### Tehtävä 2:
select game.screen_name, airport.name
from game inner join airport on airport.ident = game.location;
![image](https://github.com/user-attachments/assets/378b2b86-4be1-4048-9d0d-48daf6f25690)


### Tehtävä 3:
select screen_name, country.name
from game inner join airport on location = ident 
inner join country on airport.iso_country = country.iso_country;

![image](https://github.com/user-attachments/assets/6c8d4327-8592-4e70-8b17-3f4bfbc3caf5)


### Tehtävä 4: 
select airport.name, screen_name
from airport left join game on ident = location where name like "%Hels%" 
order by screen_name DESC;

![image](https://github.com/user-attachments/assets/118bda2d-7196-419d-abac-7fa8dde75431)


### Tehtävä 5
select name, screen_name
from goal left join goal_reached on goal.id = goal_id  left join game on game.id = game_id;

![image](https://github.com/user-attachments/assets/47cf359c-3e06-4790-889d-eca023195be8)



