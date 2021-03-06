---
title: Constants
localeTitle: Константы
---
## Константы

Константа связывает имя со значением определенного типа.

#### Пример:

```swift
let name = "Chris Lattner" 
```

Объявляем константу служебным словом `let`, потом указываем ее имя `name`, затем используем оператор присваивания `=` чтобы присвоить значение `"Chris Lattner"` константе `name`.

После того, как вы объявили константу, вам больше не нужно использовать служебное слово `let` , вы просто вызываете ее по имени.

Значение константы не может быть изменено после его присвоения. Здесь не лишним будет отметить, что компилятор в Swift достаточно сообразителен чтобы увидеть разницу между _объявлением_ константы и _присвоением_ ей значения. Посмотрим внимательнее на фрагмент кода ниже: 
```swift
let shouldWaterFreeze: Bool // (1)
if temperature < 0 {
  shouldWaterFreeze = true // (2)
} else {
  shouldWaterFreeze = false // (3)
}
```
Данный фрагмент кода корректный и компилируется без ошибок (при условии что мы уже объявили переменную `temperature` типа `Int` (целое число) и присвоили ей значение где-то ранее). Обратите внимание на то, что  мы вначале _объявили_ константу `shouldWaterFreeze` в первой строке (1), а уже потом _присвоили_ ей значение во второй или третьей строках (2) или (3).


#### Дополнительная информация:

*   [The Swift Programming Language](https://docs.swift.org/swift-book/LanguageGuide/TheBasics.html#ID310)
