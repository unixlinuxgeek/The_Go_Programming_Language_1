### 2.3 Переменные

Объявление имеет общий вид:

```
var name type expression
```

 type или expression можно не писать.

 Если опущен тип, он определяется из инициализирующего выражения. 
 Если опущено выражение, то начальным значением будет нулевое значение для
 данного типа.

 Нулевые значения:
```shell
0 для чисел
"" для строк
false для булевых переменных
nil для интерфейсов и ссылочных типов
``` 
 
Переменные уровня пакета инициализируются до начала выполнения функции main.

> Локальные переменные инициализируются тогда 
когда в процессе выполнения функции встречаются их объявления.

Сразу несколько переменных могут быть инициализированы с помощью функции
возвращающий несколько значений.

Например:
```go
var f, err = os.Open(name) // os.Open возвращает файл и ошибку
```