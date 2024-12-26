# Object-in-js
# Работа с объектами в JavaScript

В этом примере мы рассмотрим базовые операции с объектами, включая создание, изменение, удаление свойств и использование методов.

## Создание объекта

```javascript
const user = {
  name: "Alex",
  age: 25,
  isActive: true,
  greet() {
    return `Hello, my name is ${this.name}!`;
  },
};

console.log(user);
```

## Доступ к свойствам

```javascript
console.log(user.name); // Alex
console.log(user["age"]); // 25
```

## Добавление и изменение свойств

```javascript
user.email = "alex@example.com";
user.age = 26;

console.log(user);
```

## Удаление свойств

```javascript
delete user.isActive;

delete user.email;
console.log(user);
```

## Добавление свойств

```javascript
user.city = "Los Angeles";
user.phone = "123-456-7890";

console.log(user);
```

## Перебор свойств объекта

```javascript
for (const key in user) {
  console.log(`${key}: ${user[key]}`);
}
```

## Вызов метода объекта

```javascript
console.log(user.greet()); // Hello, my name is Alex!
```

## Копирование объектов

```javascript
const newUser = { ...user, city: "New York" };

console.log(newUser);
```

## Проверка наличия свойства

```javascript
console.log("email" in user); // false
console.log("phone" in user); // true
```

## Заключение

Объекты — это ключевая структура данных в JavaScript, позволяющая хранить и обрабатывать данные удобным образом.
