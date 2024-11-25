---
description: How to handle if there is some data is missing
---

# Handling With missing Data

## There are two ways to deal with this&#x20;

## 1)Drop Missing Data :-&#x20;

<mark style="color:red;">data.dropna( axis = 0, how = ' all ' )</mark>&#x20;

in axis 0 show to drop rows and 1 shows columns&#x20;

In how defines that if all data is missing then we drop that col&#x20;

<mark style="color:red;">data.dropna( subset =  \[ ' col\_name1 ' , ' col\_name2 ' ] )</mark>

It shows that if col 1 and col 2 both have any missing value the it drops those rows which does not contains the data

## 2) Filling Missing Value

<mark style="color:red;">data\[ '  col\_name' ].fillna( "Not specified" )</mark>&#x20;

<mark style="color:red;">isske aandr jiss col ka data change krna h uss col ko select krna h usske baad fillna func k aandr hume int ya sting liikhni h jo missing value ki jga pl</mark>
