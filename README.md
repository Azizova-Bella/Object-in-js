# Object-in-js
![image](https://github.com/user-attachments/assets/98746a84-7233-4d19-87cb-851d0a914d31)

# Работа с объектами в JavaScript

В этом примере мы рассмотрим базовые операции с объектами, включая создание, изменение, удаление свойств и использование методов.
![image](https://github.com/user-attachments/assets/d804f19f-e059-4bf6-8978-456abf3fb5f7)

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
![image](https://github.com/user-attachments/assets/a9033897-dc61-48f1-b1af-1a20aeb36787)


### У Object -а есть свойст, так как разделяется в 2 части. Можно посмотреть так же в код:
#### 1) Ключ
#### 2) Значение

![image](https://github.com/user-attachments/assets/dab0d602-1452-4f2f-b1a6-2549f7d26a3c)


## Доступ к свойствам

```javascript
console.log(user.name); // Alex
console.log(user["age"]); // 25
```

![image](https://github.com/user-attachments/assets/e2094de8-de82-4bd8-9808-d27ecb02ecd0)

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
![image](https://github.com/user-attachments/assets/03f2eef6-a36c-4cf7-9379-1862819d564a)

## Добавление свойств

```javascript
user.city = "Los Angeles";
user.phone = "123-456-7890";

console.log(user);
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

![image](https://github.com/user-attachments/assets/ef702e74-ecad-4159-971f-09a3db3beef2)


## Заключение

Объекты — это ключевая структура данных в JavaScript, позволяющая хранить и обрабатывать данные удобным образом.

<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/213866269-5d00981c-7c98-46d7-8a8e-16f462f15227.gif" width="200" />
  <img src="https://user-images.githubusercontent.com/74038190/213866269-5d00981c-7c98-46d7-8a8e-16f462f15227.gif" width="200" />
  <img src="https://user-images.githubusercontent.com/74038190/213866269-5d00981c-7c98-46d7-8a8e-16f462f15227.gif" width="200" />
</div>
