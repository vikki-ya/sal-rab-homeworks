# Задания к занятию «Циклы и производительность»

Напшите код решения в файле `task_4/solution.js`.

Для этого задания автотестов нет.

Изучите информацию, которая может понадобиться для выполнения заданий модуля:

[1. Начало работы на модуле](../before.md).

[2. Руководство по стилю кода](../styleguide.md).

[3. Тестирование решений](../test.md).

[4. Отправка на проверку](../after.md).

### Задание 4.1. Вывод карточек товаров

В удалённом JSON-файле `products.json` хранятся карточки товаров. Механизм получения файла уже готов, но требуется реализовать механизм вывода карточек.

### Ход решения

Закончите функцию parseProducts(). Аргументом функции parseProducts является JSON.

1. Создайте переменную data.
2. Присвойте переменной data результат преобразования аргумента в объект — JSON.parse(json).
3. Создайте переменную products.
4. Присвойте для products значение свойства data.products.
5. Верните с помощью return как результат функции parseProducts переменную products.

Создайте функцию renderProductsCards(json). Аргументом функции renderProductsCards является JSON.

1. Напишите следующий текст:
    ```javascript
    function renderProductsCards(json){
       // дальнейшие действия требуется выполнять тут
    }
    ```
2. Вызовите в функции renderProductsCards уже написанную в коде функцию clearProducts() таким образом: 
    ```javascript
    clearProducts();
    ```
3. Создайте в функции renderProductsCards переменную products.
4. Присвойте переменной products результат выполнения функции parseProducts, передав в неё JSON-аргумент функции следующим образом:
    ```javascript
    products = parseProducts(json);
    ```
5. Запишите в переменную length значение свойства products.length.
6. Напишите цикл, в котором перебираете все products от 0 до length - 1:
    ```javascript
    for (let i = 0; i < length; i += 1) {
       // место для пункта 7
    }
    ```
7. Каждую итерацию цикла вызывайте функцию addProduct, передавая элемент массива как аргумент:
    ```javascript
    addProduct(products[i]);
    ```

### Как отправить решения на проверку

1. Для этой задачи автотестов нет. При правильном выполнении выводятся карточки восьми товаров при запуске файла `index.html`:
![](../readme-img/task_4/cards.png)
2. Если обнаружены какие-то ошибки, исправьте их и проверьте решение снова.
3. Отправьте изменения в удалённый репозиторий.
4. Отправьте преподавателю на проверку ссылку на GitHub и ссылку на GitHub Pages.
