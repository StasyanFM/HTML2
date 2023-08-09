## Задача №1: проверить XML на Well formed:
### 
    <req>

        <surname>Иванов</surname>

        <name>Иван</name>

        <patronymic>Иванович</patronymic>

        <birthdate>01.01.1990</birthdate>

        <birthplace>Москва</birthplace>

        <phone>8 926 766 48 48</phone>

    </req>

### Проверка на наличие ошибок показывает отсутсвие их
![](Скрины/1.bmp)

### Удаляю лишние строки
    <req>
        <surname>Иванов</surname>
        <name>Иван</name>
        <patronymic>Иванович</patronymic>
        <birthdate>01.01.1990</birthdate>
        <birthplace>Москва</birthplace>
        <phone>8 926 766 48 48</phone>
    </req>

### Получил
![](Скрины/2.bmp)




## Задача №2: проверить JSON на Well formed:
###
    {

        "surname": ""Иванов""

        "name"": ""Иван"

        "patronymic"": ""Иванович"

        "birthdate"": ""01.01.1990"

        "birthplace"": ""Москва"

        "phone"": ""8 926 766 48 48"
    }

### При проверке получаем ошибку об отсутсвии разделительных знаков, то есть запятой ( , ) и лишние ковычки ( " )
![](Скрины/3.bmp)

### Вношу изменения   
    {
        "surname": "Иванов",
        "name": "Иван",
        "patronymic": "Иванович",
        "birthdate": "01.01.1990",
        "birthplace": "Москва",
        "phone": "8 926 766 48 48"

    }
### Получил
![](Скрины/4.bmp)