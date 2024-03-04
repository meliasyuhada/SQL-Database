<style>
    .daftar_isi {
        border: 2px;
        color: blue;
    }
</style>

<h2> Learning SQL Basic</h2>

<div class="daftar_isi"> 
<ol>
<li>
<a href="#cd">How to Create Database</a>
</li>
<li>
<a href="#sd">How to Show Databases</a>
</li>
<li>
<a href="#ct">How to Create Table</a>
</li>
<li>
<a href="#it">How to Insert Table</a>
</li>
<li>
<a href="">How to Update Table</a>
</li>
<li>
<a href="">How to Delete Table</a>
</li>
<li>
<a href="">How to Show Database and Table</a>
</li>
<li>
<a href="">How to Get Data from Table</a>
</li>
<li>
<a href="">How to Join Data Table </a>
</li>
<li>
<a href="">How to Group By Table</a>
</li>
</ol>
</div><br><br>

<div id="content">
<ol>
<li id="cd">
How to Create Database
<p><pre>CREATE DATABASE learning_sql;</pre></p>
<img src="img/create_database.png" />
</li>
<li id="sd">
How to Show Database
<p><pre>SHOW DATABASES;</pre></p>
<img src="img/show_database.png" />
</li>
<li id="ct">
How to Create Table
<p>
<pre>CREATE TABLE table_students (
    nim int(11) primary key,
    name char(20) NOT NULL,
    university char(20) NOT NULL,
    gender char(11) NOT NULL,
    age int(3) NOT NULL,
    nationality char(10) NOT NULL
    );
</pre>
</p>
<img src="img/create table.png" />

<pre>
SHOW TABLES;
</pre>

<img src="img/show table.png" />
<pre>
DESC table_students;
</pre>
<img src="img/desc tables.png" />
</li>
<li id="it">
How to Insert Table
<p>
<pre>INSERT INTO table_students VALUES
    (12340, 'Liana', 'Universitas Indonesia', 'Female', 20, 'Indonesia'),
    (12341, 'Bayu', 'Harvard University', 'Male', 21, 'Amerika Sarikat'),
    (12342, 'Garman', 'Istanbul University', 'Male', 21, 'India'),
    (12343, 'Rahel', 'Harvard University', 'Male', 20, 'Amerika Sarikat'),
    (12344, 'Xia', 'Perak University', 'Female', 20, 'Malaysia'),
    (12345, 'Zian Dewi', 'Universitas Indonesia', 'Female', 22, 'Korea');
</pre>
<img src="img/insert table.png" />
<pre>select* from table_students;
</pre>
<img src="img/select show table.png" />
</li>
</ol>
</div>
