*Принцип инверсии зависимостей (DIP)*
# Этот принцип SOLID в Java описывают так: зависимости внутри системы строятся на основе абстракций. Модули верхнего уровня не зависят от модулей нижнего уровня. Абстракции не должны зависеть от деталей. Детали должны зависеть от абстракций.
Программное обеспечение нужно разрабатывать так, чтобы различные модули были автономными и соединялись друг с другом с помощью абстракции. 
Классическое применение этого принципа — Spring framework. В рамках Spring framework все модули выполнены в виде отдельных компонентов, которые могут работать вместе. Они настолько автономны, что могут быть быть с такой же легкостью задействованы в других программных модулях помимо Spring framework.
Это достигнуто за счет зависимости закрытых и открытых принципов. Все модули предоставляют доступ только к абстракции, которая может использоваться в другом модуле.

При работе с классами которые будут связаны с другими классами, объекты не нужно напрямую передавать в другие классы, а необходимо делать это через интерфейс. Для этого в коде и используем Интерфейсы **DevClass** и **MultSumClass**.
