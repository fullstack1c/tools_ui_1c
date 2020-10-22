# Универсальные инструменты 1С для управляемых форм

[![Quality Gate Status](https://sonar.openbsl.ru/api/project_badges/measure?project=tools_ui_1c&metric=alert_status)](https://sonar.openbsl.ru/dashboard?id=tools_ui_1c) 
[![Join telegram chat](https://img.shields.io/badge/chat-telegram-blue?style=flat&logo=telegram)](https://t.me/tools_ui_1c) 
[![Last release](https://img.shields.io/github/v/release/cpr1c/tools_ui_1c?include_prereleases&label=last%20release&style=badge)](https://github.com/cpr1c/tools_ui_1c/releases/latest)
[![download](https://img.shields.io/github/downloads/cpr1c/tools_ui_1c/total)](https://github.com/cpr1c/tools_ui_1c/releases/latest/download/UI.cfe)
[![GitHub issues](https://img.shields.io/github/issues-raw/cpr1c/tools_ui_1c?style=badge)](https://github.com/cpr1c/tools_ui_1c/issues)
[![License](https://img.shields.io/github/license/cpr1c/tools_ui_1c?style=badge)](https://github.com/cpr1c/tools_ui_1c/blob/master/LICENSE)

### Поддерживаемые операционные системы

* Windows x86
* Windows x64
* Linux x64
* Linux x86

В MacOS должно работать, но не тестировалось

### Поддерживаемые клиентские приложения

* Толстый клиент управляемое приложение
* Тонкий клиент
* Web клиент(частично)

### Поддерживаемые режимы конфигурации
Модуль разрабатывается, исходя из отключенной поддержки модальности и синхронных вызовов. Должно работать во всех современных и не очень конфигурациях

### Поддерживаемые платформы
8.3.12 и выше

### Способ распространения и лицензия
Подсистема разрабатывается и распространяется под лицензией GNU General Public License v3.0. Код открыт, можно копировать и распространять кому угодно, но тоже с выкладывать в общий доступ с открытым кодом.

### На текущий момент содержит инструменты:

- **Групповая обработка справочников и документов**- Аналогична типовой обработке от 1С с диска ИТС
- **Редактор констант** - позволяет редактировать значения констант в режиме таблицы
- **Структура хранения базы данных**- Просмотр имен таблиц и их взаимосвязей с объектами метаданных.
- **Удаление помеченных объектов**- копия стандартной обработки из БСП, адаптированной для жизни вне БСП
- **Консоль запросов**- Обработка для разработки и выполнения запросов без написания дополнительных обработок. Форк https://github.com/hal9000cc/RequestConsole9000. [Лицензия GPL3](https://github.com/hal9000cc/RequestConsole9000/blob/master/LICENSE)
- **Консоль заданий**- просмотр и настройка регламентных и фоновых заданий. Форк https://github.com/kuzyara/JobsConsole2019.epf [Разрешение автора](https://github.com/kuzyara/JobsConsole2019.epf/issues/6)
- **Регистрация изменений для обмена**- Форк обработки с диска ИТС с адаптациями под подсистему
- **Поиск и удаление дублей**- Форк стандартной обработки из БСП, в которую добавлены несколько параметров выполнения замены
- **Консоль кода**- Позволяет выполнять код из предприятия без создания внешних обработок. Есть подсветка синтаксиса и минимальная контекстная подсказка.
- **Поиск ссылок на объект**- аналог стандартной обработки из меню "Все функции". 
- **Редактор реквизитов объекта**- позволяет низкоуровневое редактирование ссылочных объектов. Поддерживает редактирование движений документа. Форк обработки https://infostart.ru/public/983887/. Вырезана из https://infostart.ru/public/938606/. [Разрешение автора](http://forum.infostart.ru/forum24/topic203301/message2375899/#message2375899)
- **Консоль отчетов**- переработанная консоль компоновок с диска ИТС. Теперь ей удобнее пользоваться
- **Динамический список**- удобный просмотр списков таблиц базы из одной обработки
- **Консоль HTTP запросов**-  позволяет из 1С делать HTTP запросы. 
- **Выгрузка загрука XML с фильтрами** - Перенос информации между однородными базами данных. Форк обработки https://infostart.ru/public/1149722/ [Разрешение автора](http://forum.infostart.ru/forum15/topic229143/message2372663/#message2372663)
- **Навигатор по конфигурации**- Обработка замена стандартному меню "Все функции". Здесь же дополнительные административные фукнции будут. Форк https://infostart.ru/public/931586/. [Разрешение автора](http://forum.infostart.ru/forum9/topic202659/message2375904/#message2375904)
- **Файловый менеджер** - Обработка для удобной работы с файлами между клиентом и сервером. Передача, просмотр, удаление. На текущий момент содержит синхронные вызовы. Форк https://infostart.ru/public/1027326/. [Разрешение автора](https://github.com/cpr1c/tools_ui_1c/issues/108)
- **Конструктор регулярных выражений**-  позволяет строить сложно-структурированные выражения на основе параметрического описания, тестировать их, и в результате получить программный код 1С. На текущий момент работает только в Windows. Форк https://infostart.ru/public/592108/. [Разрешение автора](http://forum.infostart.ru/forum9/topic167495/message2389269/#message2389269)
- **Консоль вебсервисов** -Обработка для чтения и выполнения веб-сервисов на платформе 1С: Предприятие 8.3. Аналог soapUI. Обработка позволяет выполнить операцию веб-сервиса и отобразить результат в виде xml или дерева. Форк  https://github.com/ghostaz/WSReader2.git. [Лицензия GPL3](https://github.com/ghostaz/WSReader2/blob/master/LICENSE)
- **Консоль сравнения данных**- предназначена для сравнения данных, полученных из разных источников данных: информационных баз 1С 8, 1С 7.7, баз данных SQL, файлов формата CSV/TXT/DBF/XLS/DOC/XML, строки JSON, вручную заполненного табличного документа. Форк https://infostart.ru/public/581794. [Разрешение автора](http://forum.infostart.ru/forum9/topic165873/message2373325/#message2373325)
- **Информация о лицензиях 1С**-представляющая из себя обертку функций Утилиты лицензирования 1С (ring) в понятном для обычного человека виде. По сути, это GUI утилиты RING. Форк  https://infostart.ru/public/1124442/. [Разрешение автора](http://forum.infostart.ru/forum9/topic226186/message2389245/#message2389245). Для работы должна быть установлена утилита ring и ее модули license
- **Загрузка данных из табличного докумнета**-Обработка предназначена для загрузки данных в справочники и табличные части различных объектов из табличного документа. Форк обработки  https://infostart.ru/public/269425/. [Разрешение автора](http://forum.infostart.ru/forum15/topic107643/message2397121/#message2397121) 
- **Редактор JSON**- Позволяет в удобной форме редактировать строки JSON. Содержит подсветку синтаксиса JSON, редактирование в виде дерева, некоторые автоподстановки. Редактор реализован на основании библиотеки https://github.com/josdejong/jsoneditor. В Windows работает, начиная с версии платформы 8.3.14
- **Редактор HTML**- Быстрая отладка отображения HTML страниц в 1С. Представляет собой экран разбитый на 4 части, в левой части три редактора-тела HTML, CSS и JavaScript, а право - поле результата. Есть контекстная подсказка и автодополнение кода. Для редкторов кода используется библиотека https://ace.c9.io/. Незаменим, при тестировании вывода HTML в 1С, т.к. даже с платформы 8.3.14 отображение в браузере и 1С, а также в разных операционных системах может сильно отличаться. В Windows работает, начиная с версии платформы 8.3.14. [Публикация на infostart](https://infostart.ru/public/1273525/) 
- **Универсальный обмен данными в формате XML (с фильтрами и прямой загрузкой через HTTP сервис)** - Выгрузка и загрузка по правилам обмена. Форк стандартной обработки от 1С и https://infostart.ru/public/1176839/. [Разрешение](https://github.com/cpr1c/tools_ui_1c/issues/139). Добавлена возможность накладывать фильтры на выгружаемые объеты, и прямая выгрузка в базу через http сервис универсальных инструментов.  
- **Библиотека сериализации 1С**- Набор процедур и функций для сериализации/десериализации данных 1С и объектов СКД в простые структуры данных (Структура, соответствие, массив). Форк https://github.com/arkuznetsov/SerLib1C. [Лицензия MPL-2.0 License](https://github.com/arkuznetsov/SerLib1C/blob/master/LICENSE)
- **Коннектор: удобный HTTP-клиент для 1С:Предприятие 8** - В мире python очень популярна библиотека для работы с HTTP запросами - [Requests](http://docs.python-requests.org/en/master) (автор: Kenneth Reitz). Библиотека берет на себя всю рутину работы с HTTP запросами. Буквально в одну строку можно получать данные, отправлять, не заботясь о необходимости конструирования URL, кодирования данных и т.п. В общем библиотека очень мощная и проста в использовании. **Коннектор** - это "Requests" для мира 1С. Форк https://github.com/vbondarevsky/Connector. [Лицензия Apache-2.0](https://github.com/vbondarevsky/Connector/blob/master/LICENSE)

# Программный интерфейс

## Библиотека Коннектор: удобный HTTP-клиент для 1С:Предприятие 8

Доступна программно через общий модуль **УИ_КоннекторHTTP**. Подробное описание смотрите на странице библиотеки https://github.com/vbondarevsky/Connector

Пример использования:

`Результат = КоннекторHTTP.GetJson("https://api.github.com/events");`

## Библиотека сериализации 1С

Доступна программно через обработку **УИ_ПреобразованиеДанныхJSON**. Подробное описание методов смотрите на странице библиотеки https://github.com/arkuznetsov/SerLib1C

Инициализация:

`Сериализатор1С = Обработки.УИ_ПреобразованиеДанныхJSON.Создать()` 
 
Пример использования: 
 
```bsl
СериализаторJSON=Обработки.УИ_ПреобразованиеДанныхJSON.Создать();

СтруктураИстории=СериализаторJSON.ЗначениеВСтруктуру(ДанныеСохранения);
СериализуемаяСтрокаJSON=СериализаторJSON.ЗаписатьОписаниеОбъектаВJSON(СтруктураИстории);
``` 
 
### Получение структуры виртуальных таблиц запроса или менеджера временных таблиц

Необходимо в форме вычисления выражения вызвать функцию **УИ_._ВТ(ЗапросИЛИМенеджерВременныхТаблиц)**. 

Примеры использования: 

`УИ_._ВТ(Запрос)`

`УИ_._ВТ(Запрос.МенеджерВременныхТаблиц)`

### Сравнение двух таблиц значений

Необходимо в форме вычисления выражения вызвать функцию **_ТЗСр(ТаблицаБазовая, ТаблицаСравнения, СписокКолонок)**. 

Примеры использования: 

`УИ_._ТЗСр(ТаблицаБазовая, ТаблицаСравнения)` - выполнит сравнение по всем колонкам параметра ТаблицаБазовая

`УИ_._ТЗСр(ТаблицаБазовая, ТаблицаСравнения, "Номенклатура,Количество")`

### Сериализация XML в простые структуры данных(массив, структура, соответствие)

Необходимо в форме вычисления выражения вызвать функцию **_XMLОбъект(ПутьЧтения, УпроститьЭлементы)**. 

Примеры использования: 

`УИ_._XMLОбъект(ЧтениеXML)` - выполнит обход сущществующего объекта ЧтениеXML

`УИ_._XMLОбъект("C:\1.xml")` - выполнит чтение в структуры файла

`УИ_._XMLОбъект(Поток)` - выполнит чтение в структуры потока

`УИ_._XMLОбъект("C:\1.xml", Ложь)` - выполнит чтение в структуры файла без упрощения полученных структур

# Отладка

### Вызов

Необходимо в форме вычисления выражения вызвать функцию **УИ_._От(ВашаПеременнаяОбъектаОтладки,НастройкиСКД)**. Где вместо ВашаПеременнаяОбъектаОтладки нужно передать переменную, содержащую один из доступных к отладке объектов

### Логика работы

Если контекст запуска отладки является толстым клиентом открытие формы консоли происходит сразу по окончании выполнения вызова кода

Если отладка вызывается в контексте сервера или тонкого или веб клиента, необходимая информация сохраняется в справочник **Данные для отладки**. В таком случае вызов отладки проиходит потом из списка справочника "Данные для отладки". 


### Поддерживается отладка объектов:

* **Запрос**- на текущий момент отлаживаются запросы без менеджеров временных таблиц. 
Вызов отладки 

`УИ_._От(Запрос)`

* **Схема компоновки данных**- поддерживается отладка без внешних источников данных. 

Вызов отладки

`УИ_._От(СхемаКомпоновкиДанных,НастройкиСКД)` - будет вызвана отладка с переданными настройками

Или

`УИ_._От(СхемаКомпоновкиДанных)` - будет вызвана отладка с настройками по умолчанию для СКД

* **Ссылочный объект базы**- просмотр и редактирование ссылки БД

Вызов отладки

`УИ_._от(СсылкаНаОбъектБД)`

* **HTTP Запрос**- поддерживается отладка строкового и файлового содержимого запросов, а также прокси

Выззов отладки

`УИ_._От(HTTPЗапрос,СоединениеHTTP)`

# Развитие инструментов

Разработка ведется в 1С:EDT

Замечания и предложения оставляйте в разделе **issues**. 

Если кто хочет поучаствовать - добро пожаловать. Больше идей- лучше конечное решение

# Ссылки на инструмены так или иначе участвовавшие в проекте
* https://github.com/khorevaa/xml-parser- была основной для фукнции чтения XML в простые структуры данных
* https://github.com/pm74/_37583.git- На ее основе реализовывается механизм алгоритмов(хотя пока и не доделан)
