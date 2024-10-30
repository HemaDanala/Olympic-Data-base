# Olympic-Data-base
Tables 
1. create table athlete (athleteid int primary key not null,
     athletename varchar (20), gender varchar (5), dob date, countrycode varchar (5),
     foreign key(countrycode) references country(countrycode) on delete cascade on update cascade,
     eventname varchar (15),, foreign key(eventname) references event(eventname) on delete cascade on update cascade):

 2. create table site (year int primary key not null, city varchar (15), countrycode varchar (5),
     foreign key(countrycode) references country(countrycode) on delete cascade on update cascade):
    
3. create table judge (jid varchar (10) primary key not null jname varchar(20),
     igender varchar (5), nationalafiliation varchar (15), eventname varchar (15),
     foreign keyeventname) references event(eventname) on delete cascade on update cascade):
   
4. create table result (resid varchar (10) primary key not null, medaltype varchar (10), record varchar (30), athleteid int,
   foreign key(athleted) references athlete(athleted) on delete cascade on update cascade):
   
5. create table schedule (schid varchar (10) primary key not null, date date. time time, venue varchar (15)):
   
6. create table held in (schedule varchar (10), foreign key(schedule) references schedule(schid) on delete cascade on update cascade,
    eventname varchar (15), foreign key(eventname) references event(eventname) on delete cascade on update cascade):

7. create table obtained (sno int primary key not null, athleteid int. eventhame varchar (15), year int. foreign key(athleted)
   references athlete(athleted) on delete cascade on update cascade, foreign key(eventname) references event(eventname) on delete cascade on update cascade,
   foreign -key(year) references site(year) on delete cascade on update cascade):

8. create table rated by Gid varchar (10), eventname varchar (15). foreign keyjid) references judge(jid) on delete cascade on update cascade,
   foreign key(eventname) references event(eventname) on delete cascade 011 update):
