# Web3Eywa
## Софт для парсинга статистики по транзакциям в Eywa Protocol
Данный софт разработан для отслеживания статистики о транзакциях(кроссчейн свапах). Внутри чейновые свапы(пример: свап USDT на USDC внутри BSC сети) не учитываются. 

Свап EUSD считается за свап Fantom - Fantom <br />
Так же свап в/из Curve.fi Factory Plain Pool считается за свап в/из Fantom 
## Функции на данный момент
1) Показать общее количество свапов по адресу
2) Создать таблицу взаимодействия с сетями, запись в exel файл, показать свапнутый объем, всего транзакций по адресу.
3) Тоже самое что и пункт 2, только для списка адресов. Таблицы взаимодействия будут записываться в один exel файл, на разные страницы

### Консольный вывод таблицы взаимодействия
![image](https://github.com/MaloyMeee/Web3Eywa/assets/59707245/f2fa0126-104a-45f7-8c10-12ba25a99166)
### Сформированный эксель файл
![image](https://github.com/MaloyMeee/Web3Eywa/assets/59707245/7352d378-be1a-440b-9e13-71de57e07a05)

P.S Я не какой-то супер-пупер DevOps, поэтому в коде много костылей и все недочеты были заткнуты банками от энергетиков, которые пились в момент написания этого кода <br />
P.S.2 Код дико не оптимизирован, сюда можно и нужно воткнуть асинхрон/многопоточность, но мне пока лень <br />
P.S 3 Будет ребилд кода, ибо оптимизация в гробу, плюс видимо логика подсчета транзакций не правильная. В эксплорере отображаются транзакции из чейна в чейн 0, но по сути это такая транзация это завершение прошлой
