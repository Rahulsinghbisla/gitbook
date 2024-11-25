---
description: How to access data by col
---

# Access groped data

{% code fullWidth="true" %}
```markup
runs.get_group('V Kohli')
```
{% endcode %}

_<mark style="color:yellow;">delivery = pd.read\_csv('deliververies.csv')</mark>_

_<mark style="color:yellow;">runs = delivery.groupby('batsman')</mark>_

#### This is used to  get V Kohli all data so we can esaily analize it

```notebook-python
runs['batsman_runs'].sum().sort_values(ascending = False)
```

#### <mark style="color:red;">This will give total runs scored by each batsman in their descending order</mark>&#x20;

```notebook-python
mask = delivery['batsman_runs'] == 4
new_delivery = delivery[mask]
This helps us to create a new data frame of runs 
6 and then group them
```

```notebook-python
fours = new_delivery.groupby('batsman')
This will group our batsman
fours.get_group('V Kohli')['batsman_runs'].count()
This gives V Kohli total 4 its equal to no of rows

```

```notebook-python
fours['batsman'].count().sort_values(ascending=False)
This give top batsmans who hit most fours
```
