---
title: false
subtitle: false
author: false
date: false
output:
  xaringan::moon_reader:
    lib_dir: libs
    css: ["default", "assets/my-theme.css", "libs/remark-css/default-fonts.css"]
    nature:
      highlightStyle: github
      highlightLines: true
      countIncrementalSlides: false
---



#### objectives

* a practical introduction to databases
  + demystify databases
  
* focus on data structure 

---

#### terminology: what is a database?

- database (DB) is an organized collection of data

- database management system (DBMS) is software that allows interacting with the database (e.g., storing, retrieving, updating data)

.footnote[[BST 260: Introduction to Data Science](https://datasciencelabs.github.io/)]

---

#### terminology: relational database

- many types and flavors of databases: document, key-value

- relational (from relational algebra)

- RDBMS = R + DBMS

.footnote[[BST 260: Introduction to Data Science](https://datasciencelabs.github.io/)]

---

#### terminology: the language of databases

.left-column[
text
]

.right-column[
text
]


---

#### terminology: the language of databases

- SQL (Structured Query Language): language designed to interact with RDBMS

.center[
  ![sql](assets/figures/SQL-CASE-WHEN-2.png)
]

.footnote[http://razorsql.com]

---

#### RDBMS software solutions

- commercial
  + Oracle
  + Microsoft SQL Server
  + Amazon
  + others...
  
- open-source
  + MySQL
  + PostgreSQL
  + SQLite
  + others...
  
.footnote[[BST 260: Introduction to Data Science](https://datasciencelabs.github.io/)]

---

#### SQLite
  
- file-based, not client-server DB - the whole DB can live in a folder

- requires little configuration

- light but still powerful - can store and process large amounts of data

- used in most web browsers and mail clients

- consistent with database functionality across platforms

.footnote[[BST 260: Introduction to Data Science](https://datasciencelabs.github.io/)]

---

#### database table structure

<br>

.center[
  ![tr_PP](assets/figures/tableStructure.png)
]

.footnote[[BST 260: Introduction to Data Science](https://datasciencelabs.github.io/)]


---

#### database table structure: keys

<br>

.center[
  <img src="assets/figures/foreignkey.jpg" width="100%">
]

.footnote[[Foreign Keys - Intro to Relational Databases (Udacity)](https://www.youtube.com/watch?reload=9&v=fnbLMcd0FGQ)]


---

#### database structure (schema)

.center[
  <img src="assets/figures/entity-relationship-diagram.png" width="90%">
]

.footnote[Hand-crafted relational databases for fun and science, Naupaka Zimmerman, Data Carpentry, 2016-12-05]


---

#### why use a RDBMS?

- one DB vs (too) many CSV files - **complexity!**

- data size, typically when the data fits on drive but not in memory

- harness the power of SQL

- data already live in a DB

- DB provides extra tools, for example a GIS toolbox to deal with spatial data


.footnote[Introduction to Data Science: BIO 260 and CSCI E107, Harvard T.H. Chan School of Public Health]


---

#### Sycamore Creek

.center[
  <img src="assets/figures/sycamore-creek - overview.png">
]


---

#### Sycamore Creek

.center[
  <img src="assets/figures/sycamore-creek - space only.png">
]


---

#### sample sonde data

.less-left[
  <img src="assets/figures/800w_600h-HL7-HydrolabWaterQualitySonde.jpg" width="100%">
]

.more-right[
  <img src="assets/figures/example-sonde-data.png" width="110%">
]



---

#### Sycamore Creek

.center[
  <img src="assets/figures/sycamore-creek - space_sonde.png">
]


---

#### Sycamore Creek

.center[
  <img src="assets/figures/sycamore-creek - space_time.png">
]


---

#### Sycamore Creek

.center[
  <img src="assets/figures/sycamore-creek - space_time_scope.png">
]


---

#### Tres Rios Wetlands

.center[
  <img src="assets/figures/tres-rios-site-mao.png" width="45%">
]


---

#### Tres Rios raw data

<small>primary production</small>
![tr_plants](assets/figures/tr_plants.png)

<hr>
<small>transpiration</small>
![tr_PP](assets/figures/tr_primary_pro.png)

<hr>
<small>water quality</small>
![tr_water_qual](assets/figures/tr_water_qual.png)

---

#### Tres Rios database schema

.center[
  <img src="assets/figures/tres_rios_db_structure.png" width="90%">
]

---

#### Tres Rios database schema: water quality

.center[
  ![tres_rios_db_structure](assets/figures/simple_tres_rios_db_structure-water-quality.png)
]

<!--

---

#### urban Chiroptera: workflow

.center[
  ![urban-chiroptera-workflow](assets/figures/urban-chiroptera-workflow.png)
]


---

#### urban Chiroptera: schema

.center[
  ![urban-chiroptera-schema](assets/figures/urban-chiroptera-schema.png)
]

-->
