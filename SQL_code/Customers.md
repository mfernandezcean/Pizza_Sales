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


```
SELECT date, count(order_id) as ORDERS 
FROM orders 
GROUP BY 1
ORDER BY 2 desc
LIMIT 5;

```
![qwdwqdwdqwdqwdq](https://github.com/mfernandezcean/Pizza_Sales/assets/105746149/2193f436-51fd-4537-a4f7-285583e77c28)
