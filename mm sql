ADROP TABLE IF EXISTS suspects;
CREATE TABLE suspects(
suspect_id INTEGER PRIMARY KEY,
name VARCHAR(30) NOT NULL,
role VARCHAR(20),
last_seen_place VARCHAR(20),
time_seen VARCHAR(5),
carrying VARCHAR(20),
shoe_size INTEGER,
alibi VARCHAR(40),
status VARCHAR(15) DEFAULT 'suspect'
);
--INSERT record into suspect TABLE
INSERT INTO suspects
(suspect_id,name,role,last_seen_place,time_seen,carrying,shoe_size,alibi,status)
VALUES
(1,'Brian otieno','student','cafeteria','06:20','Backpack','42','NULL','suspect'),
(2,'Faith Wambui','student','cafeteria','06:35','cooler Box','38','Friend vouches for her','suspect'),
(3,'Mama Pima','cook','cafeteria','06:05','nothing','39','cooking since 5am','suspect'),
(4, 'Chege Njoroge','cleaner','cafeteria','06:50','cooler Box','42','NULL','suspect'),
(5,'Amina Hassan','student','cafeteria','06:40','umbrella','42','NULL','suspect'),
(6,'Dennis Kiorop','visitor','cafeteria','06:15','Backpack','42','Receipt from kiosk at 06:16','suspect'),
(7,'Lucy Achieng','student','cafeteria','06:55','laptop bag','40','NULL','suspect'),
(8,'Kevin Mwangi','student','library','06:30','laptop bag','42','NULL','suspect'),
(9,'Sarah Njeri','lecturer','cafeteria','07:30','cooler box','42','NULL','suspect'),
(10,'peter omondi','security','Gate','06:10','Nothing','44','on duty at the gate','suspect'),
(11,'Grace Mutheu','student','hostel','05:45','Backpack','41','roommate confirms','suspect'),
(12,'Tom barasa','visitor','cafeteria','05:50','Backpack','42','NULL','suspect'),
(13,'Janet Chebet','lecturer','lab','06:25','laptop bag','37','NULL','suspect'),
(14,'Ibrahim yusuf','student','field','06:45','Nothing','43','fitness tracker log','suspect'),
(15,'Rose Atieno','cook','cafeteria','06:00','Nothing','36','cooking since 5am','suspect');
--count all suspect;
SELECT COUNT (*) AS total_suspects FROM suspects;
--record for suspect;
SELECT * FROM suspects;
--show name and status of every suspect;
SELECT name, status FROM suspects;
--show name and role of every suspect;
SELECT name, role FROM suspects;
--seen in cafeteria;
SELECT name, last_seen_place FROM suspectS WHERE last_seen_place='cafeteria';
--select student only;
SELECT * FROM suspects WHERE role='student'; 
--display who has no alibi;
SELECT * FROM suspects WHERE alibi = 'NULL';
--whose alibi mentions cooking;
SELECT * FROM suspects WHERE alibi LIKE '%cooking%';
--role either lecturer or security;
SELECT * FROM suspects WHERE role IN ('lecturer','security');
--3 earliest sightins;
SELECT * FROM suspects ORDER BY time_seen ASC LIMIT 3;
--list each place in the file once;
SELECT DISTINCT last_seen_place FROM suspects;
SELECT alibi FROM suspects;
