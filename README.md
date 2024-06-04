# SQL-Homework-1

Inner join
select t1.*,t2.* from table1 t1 inner join table2 t2 on t1.ID = t2.ID;

Left join/ Left outer join
select t1.*, t2.* from table1 t1 left join table2 t2 on t1.ID = t2.ID;

Right join/ right outer join
select t1.ID, t1.value, t2.ID, t2.value from table1 t1 right join table2 t2 on t1.ID = t2.ID;

Simulated full outer join using union
select t1.*, t2.* from table1 t1 left join table2 t2 on t1.ID = t2.ID union select t1.ID, t1.value, t2.ID, t2.value from table1 t1 right join table2 t2 on t1.ID = t2.ID;

Cross join
select t1.*, t2.* from table1 t1 cross join table2 t2;

Equi join
select t1.*, t2.* from table1 t1 inner join table2 t2 on t1.ID > t2.ID;

Self join
select ex. name employeename, e2.name as managername from employee el inner join employee e2 on el. managerid = e2.employeeid;

Natural join
select t1.id as t1id, t1. valuel as t1value, t2.id t2id, t2.value as t2value from tablel t1 natural join table2 t2;

Join using "using" keyword
select t1.id as tiid, tl. value as tivalue, t2.id t2id, t2. value as t2value from tablel t1 inner join table2 t2 using (id);
