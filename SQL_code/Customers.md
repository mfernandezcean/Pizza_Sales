```
SELECT max(date) 
FROM orders;
```
![wdqdwwqd](https://github.com/mfernandezcean/Pizza_Sales/assets/105746149/debd9b2d-c644-49be-9ba5-d25d600ba99b)
---


```
SELECT min(date) 
FROM orders;
```
![dwqwdqwdq](https://github.com/mfernandezcean/Pizza_Sales/assets/105746149/6585a150-3fc7-4b4c-b99f-cc5dec0a513a)
---

```
SELECT  count(order_id) 
FROM orders;
```
![caascssc](https://github.com/mfernandezcean/Pizza_Sales/assets/105746149/6a66a0b2-e404-464f-9970-ab9a254f3f14)
---

```
SELECT date, count(order_id) as ORDERS 
FROM orders 
GROUP BY 1
ORDER BY 2 desc
LIMIT 5;

```
![qwdwqdwdqwdqwdq](https://github.com/mfernandezcean/Pizza_Sales/assets/105746149/2193f436-51fd-4537-a4f7-285583e77c28)
---

```
SELECT time, count(order_id) as ORDERS 
FROM orders 
GROUP BY 1
ORDER BY 2 desc
LIMIT 10;
```
![wqdwdqdwqdwqdwq](https://github.com/mfernandezcean/Pizza_Sales/assets/105746149/e72dfd4b-ba85-458f-a1e2-2126e7ee0054)
---
