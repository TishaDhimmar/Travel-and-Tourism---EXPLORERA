Hello! These queries you need to run in your MySQL Workbench

One more thing to be NOTED:
In file Conn.java , you need to change your sql username and password in line 11.

Open the folder in your Apache Netbeans or Eclipse and run the first file which is Splash.java
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
create database tms;
use tms;
show tables;

create table account(username varchar(50),name varchar(50),password varchar(50),security varchar(50),answer varchar(50));
select * from account;

create table admin(name varchar(50),username varchar(50),password varchar(50),email varchar(50),phone varchar(50),pancard varchar(50));
select * from admin;

create table customer(name varchar(50),username varchar(50),password varchar(50),email varchar(50),phone varchar(50),pancard varchar(50));
select * from customer;

create table adminlogin(username varchar(50),password varchar(50));
insert into adminlogin values('admin','admin');
select * from adminlogin;

create table bookhotel(hotelname varchar(50),name varchar(50),username varchar(50),persons varchar(50),days varchar(50),ac_nonac varchar(50),food varchar(50),totalprice varchar(50));
select * from bookhotel;

create table bookpackage(place varchar(50),name varchar(50),username varchar(50),persons varchar(50),date varchar(50),totalprice varchar(50));
select * from bookpackage;

create table hotel(name varchar(50),state varchar(50),ac varchar(50),food varchar(50),hotelcost varchar(50),image longblob);
select * from hotel;

create table package(place varchar(50),state varchar(50),price varchar(50),days_nights varchar(50),description longtext,image longblob);
select * from package;
