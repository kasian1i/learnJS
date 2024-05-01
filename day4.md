# День 4: Массивы и методы работы с ними в JavaScript

## Введение в массивы

### Создание и инициализация массивов

#### Пример создания массива

```javascript
let fruits = ['apple', 'banana', 'cherry'];
let numbers = Array(5).fill(0); // Создает массив с 5 нулями
let mixedArray = [1, 'hello', { key: 'value' }, [1, 2, 3]];
```

### Доступ к элементам массива

#### Пример доступа к элементам массива

```javascript
console.log(fruits[0]); // Выводит: apple
fruits[1] = 'mango'; // Заменяет "banana" на "mango"
```

## Обход элементов массива

### Цикл for для прохода по элементам

#### Пример

```javascript
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```

> Описание: Цикл 'for' итерирует по индексам массива от 0 до длины массива (не включая последний элемент).

### Цикл for-in для прохода по индексам массива

#### Пример прохода по индексам массива

```javascript
for (let index in fruits) {
  console.log(fruits[index]);
}
```

### Цикл for-of для прохода по значениям массива

#### Пример прохода по значениям массива

```javascript
for (let fruit of fruits) {
  console.log(fruit);
}
```

## Методы массивов

### Добавление/удаление элементов (`push`, `pop`, `shift`, `unshift`)

#### Примеры добавления/удаления элементов

```javascript
fruits.push('orange'); // Добавляет "orange" в конец массива
fruits.pop(); // Удаляет последний элемент массива
fruits.shift(); // Удаляет первый элемент массива и возвращает его
fruits.unshift('kiwi'); // Добавляет "kiwi" в начало массива
```

## Итерационные методы (`forEach`, `map`, `filter`, `reduce`)

### forEach

#### Пример forEach

```javascript
fruits.forEach(function (item) {
  console.log(item);
});
```

### map

#### Пример map

```javascript
let lengths = fruits.map(function (item) {
  return item.length;
});
console.log(lengths); // Выводит массив длин элементов
```

### Методы поиска (`find`, `indexOf`)

#### Пример `find`, `indexOf`

```javascript
let found = fruits.find(function (element) {
  return element === 'cherry';
}); // Находит "cherry" в массиве
```

## Многомерные массивы

### Работа с многомерными массивами

#### Пример работы с многомерным массивом

```javascript
let matrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
];
console.log(matrix[0][1]); // Выводит: 2
```
