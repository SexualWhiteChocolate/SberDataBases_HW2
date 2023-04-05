# SberDataBases_HW2

Использовать будем стандартный датасет Titanic Dataset. Записи в этом датасете имеют следующий вид:

Пример элемента данных            |  Состояние базы данных
:-------------------------:|:-------------------------:
![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image1.jpg)  |  ![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image.png)

# Операции над данными

## Read

Определим процент выживших:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image2.jpg)

Найдем распределение количества пассажиров по классу билета:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image3.jpg)

## Update

Уточним класс билета у Mr. Owen Harris Braund:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image4.jpg)

А также его возраст:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image5.jpg)

## Create & Delete

Добавим Mr. Owen Harris Braund-а младшего:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image5.jpg)

Найдем теперь всех Harris Braund-ов:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image6.jpg)

Удалим последнее изменение:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image7.jpg)

## Индекс

Чтобы найти всех пассажиров младше пяти лет, нам понадобилось обработать все документы, ведь возраста неиднексированы и записи не упорядоченны:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image8.jpg)

После внедрения индекса тот же запрос обрабатывается просматривая только столько записей, сколько выдается всего по итогу:

![](https://github.com/SexualWhiteChocolate/SberDataBases_HW2/blob/main/image9.jpg)

Итого, действительно, индексирование и упорядочивание данных значительно облегчает поиск по данным при малых затратах на хранение. Данные, которые я выбрал, оказались достаточно скудны, индекс по классу или признаку выжил/нет будет мало полезна, индекс по имени работает плохо. Пожалуй, единственный индекс, который имеет смысл - это, пожалуй, только выбранный, для какой-нибудь статистики по возрасту пассажиров Титаника, например.
