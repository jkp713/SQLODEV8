# SQLODEV8

CREATE TABLE employee (
	id INTEGER PRIMARY KEY,
	name VARCHAR(50) NOT NULL,
	birthday DATE,
	email VARCHAR(100)
);

SELECT * FROM employee;

insert into employee (id, name, birthday, email) values (1, 'Roxi', '1974-07-31', 'rhathorn0@mail.ru');
...
insert into employee (id, name, birthday, email) values (50, 'Delmor', '1998-02-23', 'dforth1d@live.com');

SELECT * FROM employee;

UPDATE employee
SET name = 'denemeler'
WHERE id>0 AND id<6
RETURNING *;

SELECT * FROM employee;

DELETE FROM employee
WHERE id>45 AND ID<51
RETURNING *;
