## Описание

Вкратце
Шаблон применяется для минимизирования использования памяти или вычислительной стоимости за счёт общего
использования как можно большего количества одинаковых объектов.

Или

«Приспособленец» — это объект, минимизирующий использование памяти за счёт общего с другими,
такими же объектами использования как можно большего объёма данных. Это способ применения многочисленных
объектов, когда простое повторяющееся представление приведёт к неприемлемому потреблению памяти.

**Цель**

Оптимизация работы с памятью путём предотвращения создания экземпляров элементов, имеющих общую сущность.

**Описание**

Flyweight используется для уменьшения затрат при работе с большим количеством мелких объектов. При проектировании
приспособленца необходимо разделить его свойства на внешние и внутренние. Внутренние свойства всегда неизменны,
тогда как внешние могут отличаться в зависимости от места и контекста применения и должны быть вынесены
за пределы приспособленца.

Flyweight дополняет шаблон Factory Method таким образом, что при обращении клиента к Factory Method для
создания нового объекта ищет уже созданный объект с такими же параметрами, что и у требуемого, и возвращает
его клиенту. Если такого объекта нет, то фабрика создаст новый.

