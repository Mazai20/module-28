## Project of testing <a href = "https://samara.holodilnik.ru/" target="_blank">Holodilnik</a> website ©
### Project structure:

### Папка tests:

<strong>test_authorization</strong> - Тестируем Регистрацию и Авторизацию на сайте
<br><strong>test_main_page</strong> - Тестируем Открытие сайта, Каталог товаров и Элементы на главной странице сайта
<br><strong>test_filter_sort</strong> - Тестируем работу Фильтра и Сортировку товаров
<br><strong>test_card_basket</strong> - Тестируем Карточки товаров на странице и Функционал Корзины
<br><strong>Notebook.json</strong> - Файл для сохранения результатов тестов

### Папка pages:

<strong>API_RegMail</strong> - GET-запросы к виртуальному почтовому ящику (1secmail.com) для получения валидного Email и кода для регистрации на сайте.
<br><strong>Locators</strong> - локаторы XPath и CSS на web-элементы сайта
<br><strong>PageAutho</strong> - функции-обёртки для локаторов, распределённые по классам в зависимости от тематики тестов
<br><strong>BaseApp</strong> - функции для применения к локаторам явных ожиданий, получения главной страницы сайта и пути текущей страницы
<br><strong>Config</strong> - исходные статические данные
<br><strong>Settings</strong> - сохранённые, в процессе теста, виртуальные учётные данные
<br><strong>check_count</strong> - файл для нумерации тестов при сохранении результатов в файл Notebook.json. Для обнуления счётчика нужно указать значение = 0.


### Папка screenshots:
В папке сохраняются скриншоты некоторых страниц.

### Папка allure-report:
Отчёт по пройденным тестам.
<br><img src="https://antonov21vek.ru/data/documents/allure_report_1.jpg" width="500" height="230"><img src="https://antonov21vek.ru/data/documents/allure_report_2.jpg" width="500" height="230">


  
<br><strong>ВНИМАНИЕ!!!
<br>Тесты настроены на запуск через Run!</strong>
<br>При запуске через CMD из Terminal, файлы для хранения учётных данных не будут сохраняться в нужных папках,
что приведёт к ошибке во время выполнения теста.
<br>При необходимости запуска из Terminal можно закомментировать строки, сохраняющие данные в файл, в т.ч. в файле conftest.py, но при этом, тесты авторизации могут не работать, так как для них нужен доступ к сохранённым значениям в файле Settings.py.
<br><strong>Также на сайте есть Антиробот.</strong> При поточном запуске тестов, возможна блокировка сайта. Лимит на авторизацию - 10 раз.

 
 
