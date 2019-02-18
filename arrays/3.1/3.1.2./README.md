## Задача 2. Сортировка массива вручную.
### Описание

Вы пишете программу анализа цен в интернете. Ваш анализатор получил “сырой” список товаров. Вам необходимо отсортировать этот список в порядке увеличения цен.

Массив на вход- массив объектов, типа “Продукт” с полями- “Имя, цена, описание”.

Массив на выход- отсортированный по возрастанию цены массив продуктов.

Нужно учесть: 

* массив на вход может быть очень большим, а значит алгоритм ручной сортировки должен быть эффективнее, чем “сортировка пузырьком”. 
* цены могут совпадать.


### Реализация
1. Создаем объект для продуктов. 
 ```
public class Product {
    private String name;
    private int price;
    private String description;

    public Product(int price, String name, String description) {
       this.name = name;
       this.price = price;
       this.description = description;
    }
    // getters and setters
 }
 ```
2. Пишем метод сортировки, который при входе получает список продуктов (массив объектов, типа “Продукт”).
```
mySort(Prodcut[] products)
```
3. Пишем алгоритм сортировки. 
Можно выбрать один из известных алгоритмов, например:

``` Merge Sort, Quick Sort ```

или создать самому.
Просмотрите все возможные алгоритмы сортировки, выберите один из них. 
Напишите метод ```mySort(Prodcut[] products)``` по выбранному алгоритму.

### Дополнительно 

Изучите  готовые решения от Java. Будет полезно узнать, какой алгоритм сортировки использует Java и почему.  Для практики примените Comparator и передайте массив вместе с компаратором методу сортировки (так же можно использовать Comparable интерфейс в классе).
  
  Полезные ссылки:
	[Comparator](https://docs.oracle.com/javase/7/docs/api/java/util/Comparator.html),
	[Arrays.sort](https://docs.oracle.com/javase/7/docs/api/java/util/Arrays.html#sort%28T%5B%5D,%20java.util.Comparator%29),
	[Comparable](https://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html).
