This is the first sample file for git commands practice
```
CREATE TABLE country (
	id SERIAL PRIMARY KEY,
	name VARCHAR(50),
	population INTEGER, 
	area_sqkm INTEGER
);

CREATE TABLE city (
	id SERIAL PRIMARY KEY, 
	name VARCHAR(50),
	country_id INTEGER REFERENCES country(id)
);

CREATE TABLE people (
	id SERIAL PRIMARY KEY,
	name VARCHAR(50),
	age INTEGER,
	height INTEGER,
	city_id INTEGER REFERENCES city(id)
);
```
