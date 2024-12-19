# Коллекция архивов WARC
## Описание коллекции

Данный архив представляет собой коллекцию архивированных сайтов, посвященных российским
экстремальным зимним фестивалям. Это уникальный сборник, который можно пополнять и
анализировать, обеспечивая сохранение культурной информации и предоставление ресурсов для
различных целей. Он обеспечивает стабильный и надежный источник информации о развитии
зимних спортивных фестивалей в России.
Этот архив не только сохраняет прошлое, но и служит основой для изучения и развития будущих
зимних фестивалей в России.

## Cайты:
Коллекция включает архивы следующих сайтов:

- elbrus.redfox.ru
- grelkafest.com
- newstarcamp.com

## Метод и технология сбора архивов
Архивы были собраны с использованием следующих инструментов и технологий:

Инструмент: Wpull, Metawarc, ArchiveToday

Формат архива: WARC (Web ARChive)

Метод сбора: Полное сканирование сайтов с сохранением всех страниц, изображений, скриптов и других ресурсов.

Дата сбора: 18 декабря 2024 года

## Контакты
**Автор:** Латыпов Глеб
**Email:** gl.latypov@mail.ru
**GitHub:** (https://github.com/ostpanther)

## Условия использования
Коллекция распространяется под открытой лицензией *Creative Commons Zero v1.0 Universal*. Это означает, что данный репозиторий можно свободно использовать, изменять и распространять данные, при условии указания авторства и сохранения лицензии.

## Описание метаданных архивов и самих архивов
- В каталоге *archive* содержаться архивы сайтов (warc-файлы), metawarc-файлы(папки пусты, поскольку размер слишком большой), а также скриншоты с сайта ArchiveToday

- В файле *описание архива.docx* вы можете найти описание всех архивов

- С более содержательными данными вы можете ознакомиться в катлогах с окончанием *_metawarc*
- В файле code.ipynb описывается весь код 

P.s.: 
Данные разбиты по файлам. Если вас интересует содержание всех данных, то есть специально созданный файл, хранящий в себе скомбинированные результаты в  *_metawarc/combined_results.txt*

**1. elbrus.redfox.ru**
Размер архива:
* Общий размер: 643.68 MB
* Количество записей: 1935

**Особенности**
- Сайт содержит статические страницы и изображения.
- Архив включает все страницы, доступные на момент сбора.

**2. grelkafest.com**
Размер архива:
* Общий размер: 3.77 MB
* Количество записей: 21

**Особенности**
- Сайт содержит минимальное количество ресурсов.
- Основной тип контента — HTML-страницы.

**3. newstarcamp.com**
Размер архива
* Общий размер: 1.18 GB
* Количество записей: 2291

**Особенности**
- Сайт содержит большое количество статей и изображений.
- Архив включает все страницы и ресурсы, доступные на момент сбора.
- Наиболее полный архив из всех представленных 

## Пример команд для анализа архивов 
Для анализа архивов использовались следующие команды:

* Metadata command
`!metawarc metadata newstarcamp.ru/newstarcamp.ru.warc.gz > newstarcamp_metawarc/metadata_results.txt`

* Analyze command
`!metawarc analyze newstarcamp.ru/newstarcamp.ru.warc.gz > newstarcamp_metawarc/analyze_results.txt`

* Index command
`!metawarc index newstarcamp.ru/newstarcamp.ru.warc.gz > newstarcamp_metawarc/index_results.txt`

* Export command 
`!metawarc export newstarcamp.ru/newstarcamp.ru.warc.gz --output newstarcamp_metawarc/exported_content > grelkafest_metawarc/export_results.txt`

* List command 
`!metawarc list -m newstarcamp.ru/sitearchive-newstarcamp.ru.db > newstarcamp_metawarc/list_results.txt`

* Dump command
`!metawarc dump -m newstarcamp.ru/sitearchive-newstarcamp.ru.db > newstarcamp_metawarc/dump_results.txt`
