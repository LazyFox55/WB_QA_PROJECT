# SQL запросы — Wildberries.ru (учебный пример)

Данные запросы являются примерами того, как QA-инженер может проверять данные в базе данных (если есть доступ).

---

### 1. Поиск товаров по цене (меньше 1000)
```sql
SELECT id, name, price 
FROM products 
WHERE price < 1000 
ORDER BY price ASC;
```

### 2. Подсчет количества товаров в категории
```sql
SELECT category_name, COUNT(*) as product_count
FROM products
GROUP BY category_name;
```

### 3. Поиск пользователей, зарегистрированных за последний месяц
```sql
SELECT email, registration_date
FROM users
WHERE registration_date >= '2026-05-01';
```
