https://inna-malina.github.io/nevtrip-little-site/
### Вёрстка страницы
Вёрстка страницы по [макету](https://www.figma.com/file/JyFQcxiynMH1i5ViWz4qi0/Layout-test-task?node-id=0%3A1) - выполнено [ссылка на вёрстку](https://inna-malina.github.io/nevtrip-little-site/)

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
* и добавила box-sizing: border-box чтоб padding не добавлял ширину блоку.
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
###
