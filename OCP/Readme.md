*Принцип открытости/закрытости (OCP)*
# Этот принцип ёмко описывают так: программные сущности (классы, модули, функции и т.п.) должны быть открыты для расширения, но закрыты для изменения.
Это означает, что должна быть возможность изменять внешнее поведение класса, не внося физические изменения в сам класс. Следуя этому принципу, классы разрабатываются так, чтобы для подстройки класса к конкретным условиям применения было достаточно расширить его и переопределить некоторые функции.
Поэтому система должна быть гибкой, с возможностью работы в переменных условиях без изменения исходного кода.
1. В текущей работе калькулятора имеются методы вычисления суммы и умножения, при нахождении их в одном классе они нарушают этот второй принцип.
2. Для того чтобы исправить это, необходимо использовать "полиморфизм" и абсстрактыне классы, для этого будем использовать интерфейс.
3. Мы создаем отдельные классы которые будт работать через интерфейс, в каждом из них будет только одно действие, умножение и сложение
4. В свою очередь класс для деления останется в отдельно м классе **и будет соответствовать принципу разделения S**

I. Создадим интрефейс в который вставим метод который потом будем перегружать в дочерних классах. 

II. Меняем  имена классов на узкоспециализированный, и включаем реализацию интерфеса.

III. В дальнейшем при расширении функционала нам надо будет только создавать дополнительный наследованный класс с новым интерфейсом.
