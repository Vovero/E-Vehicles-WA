# Project_1select * from electric_vehicle_population_data;


-- identifiying distinct State
select distinct State
From electric_vehicle_population_data;


-- identifiying distinct County in washington state
select distinct County
From electric_vehicle_population_data;

-- identifiying distinct make
select distinct Make
From electric_vehicle_population_data;

-- identifiying distinct Make & Model
select distinct Make, Model
From electric_vehicle_population_data;


-- identifiying distinct Make, Model & model year
select distinct Make, Model, `model year`
From electric_vehicle_population_data;

-- identifiying E-vehicle with battery
select county, City, State, Make, Model, `Model year`, `Electric Vehicle Type`
From electric_vehicle_population_data
where `Electric Vehicle Type` like '%battery%';

-- identifiy electric range greater than or equal to 200
select county, City, State, Make, Model, `Model year`, `Electric Vehicle Type`, `Electric Range`
From electric_vehicle_population_data
where `Electric Range` >= "200" ;

-- identifiy electric range less than 200
select county, City, State, Make, Model, `Model year`, `Electric Vehicle Type`, `Electric Range`
From electric_vehicle_population_data
where `Electric Range` < "200" ;


-- identifiying E vehicle Tyep hybrid 
select county, City, State, Make, Model, `Model year`, `Electric Vehicle Type`
From electric_vehicle_population_data
where `Electric Vehicle Type` like '%plug%';

