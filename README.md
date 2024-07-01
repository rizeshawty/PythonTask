# Поиск чисел с четырьмя делителями
**Напишите программу, которая ищет среди целых чисел, принадлежащих числовому отрезку [185 311; 185 330], числа, имеющие ровно четыре различных натуральных делителя.** 

*Для каждого найденного числа запишите эти четыре делителя в четыре соседних столбца на экране с новой строки. Делители в строке должны следовать в порядке возрастания.*

## Содержание
- [Циклы](https://wiki.python.org/moin/ForLoop)
- [Команда](https://www.vstu.ru/university/personalii/zhdanov_aleksey_andreevich/)
  
## Использование
Может быть полезна в областях математики, алгоритмов, и исследования чисел. Программа позволяет находить числа в заданном диапазоне с определенным количеством различных натуральных делителей. Конкретно в данном случае, программа находит числа с ровно четырьмя различными натуральными делителями в диапазоне от 185 311 до 185 330, выводит их делители в порядке возрастания на экране.

```python
for otrezok in range(185311, 185330+1):
    massiv = []
    for delenie in range(2, 185330+1):
        if otrezok % delenie == 0:
            massiv.append(delenie)
            if len(massiv) == 4:
                print(*massiv)
```

### Требования
Для установки и запуска, необходим [Python](https://www.python.org/downloads/).

## Deploy и CI/CD
Anaconda, Sublime Text, Atom, VS Code, Google Colab, 
[еще...](https://realpython.com/run-python-scripts/)

## Contributing
Для улучшения кода рекомендуется обращаться через социальные сети.

### Для чего
Данный проект был разработан в рамках изучения системного программирования и выполнения предложенного задания.

## Источники
Если вы чем-то вдохновлялись, расскажите об этом: где брали идеи, какие туториалы смотрели, ссылки на исходники кода. 
