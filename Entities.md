# **Entities**

## 1. Soldier
 - id INT, NOT NULL, PK
 - first_name CHAR, NOT NULL
 - last_name CHAR, NOT NULL
 - patronymic CHAR, NOT NULL
 - military_call_sign CHAR, NOT NULL
 - date_of_birth DATE, NOT NULL

 ## 2. Military ID
 - id, INT, NOT NULL, PK
 - name CHAR, NOT NULL
 - branch_of_the_army INT, NOT NULL, FK
 - rank INT, NOT NULL, FK

 ## 3. Branch of the army
 - id, INT, NOT NULL, PK
 - name_of_the_branch CHAR, NOT NULL
 - military_specalization CHAR, NOT NULL

 ## 4. Rank
 - id, INT, NOT NULL, PK
 - name_of_the_rank, CHAR, NOT NULL
 - description, CHAR, NOT NULL

 ## 5. Weapon 
 - id, INT, NOT NULL, PK
 - serial_number, CHAR, NOT NULL
 - type_of_ammo, CHAR, NOT NULL
 - model, CHAR, NOT NULL
 - manufacturer, INT, NOT NULL, FK
 - holder, INT, FK

 ## 6. Military Equipment
 - id, INT, NOT NULL, PK
 - serial_number, CHAR, NOT NULL
 - model, CHAR, NOT NULL
 - manufacturer, INT, NOT NULL, FK
 - holder, INT, FK

 ## 7. Manufacturer
 - id, INT, NOT NULL, PK
 - name, CHAR, NOT NULL
 - country, CHAR, NOT NULL

 ## 8. Report
 - id, INT, NOT NULL, PK
 - report_topic, CHAR, NOT NULL
 - description, CHAR, NOT NULL
 - date, DATE, NOT NULL
 - author, INT, NOT NULL, FK

 ## 9. Speciality
 - id, INT, NOT NULL, PK
 - name, CHAR, NOT NULL
 - description, CHAR

 ## 10. Mility Award
 - id, INT, NOT NULL, PK
 - name, CHAR, NOT NULL
 - description, CHAR