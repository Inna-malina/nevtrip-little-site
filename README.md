[Ссылка на моё портфолио] (https://inna-malina.github.io/my_cv/)
### Вёрстка страницы
Ссылка на свёрстанный макет [ссылка на вёрстку](https://inna-malina.github.io/nevtrip-little-site/)
Ссылка на страницу с кодом [здесь](https://github.com/Inna-malina/nevtrip-little-site)

### Таблица на странице
Если таблица не помещается в ширину дисплея, то это решается просто. Саму таблицу нужно обернуть в контейнер
и на определённой ширине задать ему горизонтальный скролл. Тогда при уменьшении экрана таблица будет скроллица, а остальной макет не будет разваливаться.
Как вариант можно посмотреть [здесь](https://github.com/Inna-malina/neva-trip-table)
Но, тот вариант вёрстки, который вы предоставили, сам по себе содержит некоторые недочёты, которые дают скролл и без таблицы.
* заданы два разных width у основного блока
* отсутствует мобильная вёрстка

Как это решается:
* на ширине 600рх я создала медиазапрос
* ширину основного содержимого сделала 95%
* и добавила box-sizing: border-box, чтоб padding не добавлял ширину блоку.
```
  @media screen and (max-width: 600px) {
    .table-wrap {
        overflow-x: scroll;
        width: 100%;
    }

    .blog {
        position: relative;
        margin: 0 auto;
        padding: 20px 15px;
        max-width: 95%;
        box-sizing:border-box;
        background-color: #fff;
    }
  }
```
### Билеты на событие
Папки с кодом находятся [здесь](https://github.com/Inna-malina/neatrip-ticket-on-events), посмотреть как работает сама страница и формируется таблица можно посмотреть [здесь](https://inna-malina.github.io/neatrip-ticket-on-events/)
На данный момент я не умею работать с БД и отправлять данные, полученные из формы в php таблицы, если бы вы в вакансии указали, что нужны такие знания,как php, sql, google-таблицы, то скорее всего я бы не откликалась.
Но так какэтот момент я увидела, когда практически всё ТЗ было выполнено, то решила не бросать задачи, а сформировать таблицу при помощи JavaScript. Но я понимаю, что скорее всего это совсем не то, что вы ожидали увидеть.
### Время из A в B
Папки с кодом находятся [здесь](https://github.com/Inna-malina/nevatrip-ticket-on-ship), а посмотреть, как работает страница можно [здесь](https://inna-malina.github.io/nevatrip-ticket-on-ship/)
