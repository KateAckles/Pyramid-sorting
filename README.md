На входе: Массив
На выходе: Массив
Что делает:Пирамида — двоичное дерево, в котором значение каждого элемента больше либо равно значений дочерних элементов.
            Заполнив дерево элементами в произвольном порядке, можно легко его отсортировать (легче, чем исходный список элементов), превратив в пирамиду.
            Самый большой элемент пирамиды находится в её вершине.
            Отделяем вершинный элемент, и записываем его в конец результирующего массива.
            На место вершинного элемента записываем элемент из самого нижнего уровня дерева.
            Восстанавливаем (пересортировываем) пирамиду.
            Самый большой элемент из оставшихся снова в вершине. Снова отделяем его и записываем его в качестве предпоследнего элемента результата, и так далее...
            Весь фокус алгоритма в том, что пирамида без дополнительных затрат хранится прямо в исходном массиве. По мере того, как размер пирамиды уменьшается, она занимает всё меньшую часть массива, а результат сортировки записывается начиная с конца массива на освободившиеся от пирамиды места.
