---
layout: post
title: Java 8 Streams / SQL
tags:
  - java
  - stream-api
  - sql
main-class: stream-api
categories: 
  - stream-api
---

**Друзья, всем привет!**

В статье с [javacodegeeks.com](https://www.javacodegeeks.com/2016/04/10-sql-tricks-didnt-think-possible.html) нашел таблицу, в которой провели аналогию между методами StreamApi и SQL. Как мне показалось, полезная для понимания StreamApi табличка. *Увеличивает количество ассоциативных связей в мозгу )))*. При условии, что вы знакомы с SQL. 

|SQL           |Java      |
|--------------|----------|
|TABLE         |Stream    |
|SELECT        |map()     |
|DISTINCT      |distinct()|
|JOIN          |flatMap() |
|WHERE / HAVING|filter()  |
|GROUP BY      |collect() |
|ORDER BY      |sorted()  |
|UNION ALL     |concat()  |

В неё можно добавить еще пару строк, например:

|SQL           |Java      |
|--------------|----------|
|COUNT()       |count()   |
|MIN()         |min()     |
|MAX()         |max()     |

Грубо говоря, StreamApi это еще один вариант решения уже известных задач над данными - объединение данных из разных источников, наложение условий и фильтрация, сортировка, отображение одних значений на другие и.т.д.

PS. Я не нашел в SQL аналогов метода reduce и peek. Возможно, в StreamApi нет аналогов некоторым конструкциям из SQL.
