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


# Методы Object 

## 1. Object.values()

```javascript 
const values = Object.values(person);
console.log(values);
// Output: [ "Alice", 25, "Developer" ]
```
## 2. Object.keys()

```javascript
const keys = Object.keys(person);
console.log(keys);
// Output: [ "name", "age", "occupation" ]

```

## 3. Object.entries()

```javascript
const entries = Object.entries(person);
console.log(entries);
// Output: [ ["name", "Alice"], ["age", 25], ["occupation", "Developer"] ]
```

## Доступ к свойствам

```javascript
console.log(user.name); // Alex
console.log(user["age"]); // 25
```

![image](https://github.com/user-attachments/assets/093fd223-2528-4472-a954-e768a130dac6)


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

# For ...in Example 
```javascript
function hasKey(obj, value){
    for(let key in obj){
        if (key == obj[key])
            return true
    }
    return false
}
console.log(hasKey({ a: 44, b: 45, c: 46 },"d")); // false
```

![image](https://github.com/user-attachments/assets/ba77f9d6-7b74-49e2-a533-65fe76257d22)

## Проверка наличия свойства

```javascript
console.log("email" in user); // false
console.log("phone" in user); // true
```

# DESTRUCTURING - берет ключ от обьекта и найдёт значение 
## Значение перемещается в другом перемене.

![image](https://github.com/user-attachments/assets/ef702e74-ecad-4159-971f-09a3db3beef2)


## Заключение

Объекты — это ключевая структура данных в JavaScript, позволяющая хранить и обрабатывать данные удобным образом.

![Alt Text](https://camo.githubusercontent.com/514f682a0b43a9422eee5d9e1d81ef2b7c866247575a96f1080913870d87f0e9/68747470733a2f2f63646e612e61727473746174696f6e2e636f6d2f702f6173736574732f696d616765732f696d616765732f3032382f3130322f3035382f6f726967696e616c2f706978656c2d6a6566662d6d61747269782d732e6769663f31353933343837323633)


