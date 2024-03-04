<center><h2> Learning SQL Basic</h2></center>

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
<a href="#adc">How to Add Column</a>
</li>
<li>
<a href="#dc">How to Drop Column</a>
</li>
<li>
<a href="#mc">How to Modify Column</a>
</li>
<li>
<a href="#cc">How to Change Column</a>
</li>
<li>
<a href="#ut">How to Update Table</a>
</li>
<li>
<a href="#dt">How to Delete Table</a>
</li>
<li>
<a href="#rt">How to Rename Table</a>
</li>
<li>
<a href="sd">How to Select</a>
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
<li id="adc">
How to Add Column
<p>
<pre>
ALTER TABLE table_students ADD level int(3);
</pre>
<img src="img/add-colums.png" />
<pre>desc table_students;
</pre>
<img src="img/desc_addc.png" />
</li>

<li id="dc">
How to Drop or Delete Column
<p>
<pre>
ALTER TABLE table_students DROP COLUMN level;
</pre>
<img src="img/drop-column.png" />
<pre>desc table_students;
</pre>
<img src="img/desc-dc.png" />
</li>

<li id="mc">
How to Modify Column
<p>
<pre>ALTER TABLE table_students MODIFY nim BIGINT;
</pre>
<img src="img/modify-column.png" />
<pre>desc table_students;
</pre>
<img src="img/desc-m.png" />
</li>

<li id="cc">
How to Change Column
<p>
<pre>ALTER TABLE table_students CHANGE nationality kebangsaan char(10);
</pre>
<img src="img/change-column.png" />
<pre>desc table_students;
</pre>
<img src="img/desc-cc.png" />
</li>

<li id="ut">
How to Update Table
<p>
<pre>UPDATE peserta SET university = 'Universitas Gajah Mada' WHERE name = 'Xia';
</pre>
<img src="img/update-column.png" />
<pre>select* from peserta;</pre>
<img src="img/select-update.png" />

<pre>UPDATE peserta SET kebangsaan = 'Jakarta' WHERE name = 'Zian Dewi' OR nim = 12344;</pre>
<img src="img/update2.png" />

<pre>select* from peserta;</pre>
<img src="img/select-update2.png" />
</li>

<li id="rt">
How to Rename Table
<p>
<pre>ALTER TABLE table_students RENAME TO peserta;
</pre>
<img src="img/rename-table.png" />
<pre>show tables;
</pre>
<img src="img/show-rt.png" />
</li>

<li id="sd">
How to Select
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
