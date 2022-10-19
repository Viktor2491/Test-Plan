# План тестирования возможности записи на обучение профессии "Тестировщик ПО".

# Перечень автоматизируемых сценариев:

Тестируемая форма для записи на обучение профессии "Тестировщик" находится на странице https://netology.ru/programs/qa (далее - "Страница"), попасть на которую можно используя указанные ниже пути :

1.Путь "Каталог курсов"
Переход с главной страницы Сайта в меню "Каталог курсов" -> меню "Программирование" -> вкладка "Тестировщик ПО"

1.Путь "Направление обучения"
Переход с главной страницы Сайта в меню "Программирование" расположенное в блоке "Направление обучения" -> блок "Программирование" -> вкладка "Тестировщик ПО"

1.Путь "Раскройте свои сильные стороны"
Нажать на кнопку "Выбрать курс", расположенную на главной странице в блоке "Раскройте свои сильные стороны" -> вкладка "Тестировщик ПО"

1.Путь "Полный каталог курсов"
Переход с главной страницы Сайта в меню "Каталог курсов" -> кнопка "Полный каталог курсов" -> вкладка "Тестировщик ПО"

1.Путь "Финальный блок"
Выбрать меню "Программирование" в самом нижнем блоке страницы -> вкладка "Тестировщик ПО"

# Тестовые сценарии:

* Позитивные: *
1. валидный телефон и минимально короткое имя, например "Ян"
1. валидный телефон и сложное имя через дефис, например "Анна-Мария"
1. валидный телефон и стандартное имя, например "Александр"
1. валидный телефон и сложное имя через пробел, например "Олег Иванов"
1. валидный телефон и имя, перед которым несколько пробелов
1. валидный телефон и имя, в котором есть буква "ё"

* Негативные: *
1. с пустыми полями Имя и Телефон
1. с валидным именем но пустым полем телефона
1. с валидным телефоном но пустым полем имени
1. с валидным именем но невалидным телефоном (цифр в номере меньше установленного)
1. с валидным именем но невалидным телефоном (цифр в номере больше установленного)
1. с валидным именем но невалидным телефоном (буквы вместо цифр)
1. с валидным именем но невалидным телефоном (все цифры в номере нули)
1. с валидным именем но невалидным телефоном(в поле "телефон" пробел)
1. с валидным именем, но невалидным именем (сочетание цифр и символов в номере)
1. с валидным телефоном но невалидным именем (имя написано латиницей)
1. с валидным телефоном но невалидным именем (имя написано цифрами)
1. с валидным телефоном но невалидным именем (имя содержит недопустимые символы)
1. с валидным телефоном но невалидным именем (имя превышает допустимое количество символов)
1. с валидным телефоном но невалидным именем (пробел в поле "Имя")

# Перечень используемых инструментов:

1. IntelliJ IDEA 2021.1.3 - функциональная среда разработки, подходящая для многих языков программирования;
1. Java 11 - объектно-ориентированный язык программирования, оптимальный для написания понятных и наглядных автотестов;
1. Gradle - мощная и простая система автоматической сборки проектов;
1. Selenide - изящный API, простота использования;
1. JUnit 5 - среда модульного тестирования для языка программирования Java;
1. Lombok - плагин для автоматической генерации кода, позволяет сократить количество кода;
1. Git - система контроля версий, позволяет фиксировать изменения в коде, быстро "откатить" изменения назад, сохранять предыдущие версии.

# Перечень необходимых разрешений/данных/доступов:

1. Разрешение на проведение тестирования и автоматизацию.
1. Получение доступа к API и БД для проверки результатов выполнения тестов.
1. Тех. документация, чтобы понимать какие данные будут являться валидными, а какие - нет.

# Перечень и описание возможных рисков при автоматизации:

1. Отсутствие технической документации.
1. Возможное изменение верстки (поведения) и селекторов страницы.
1. Возможные проблемы при соединении к продакшн или тестовому стенду.
1. Тестовые данные могут попасть в реальную базу данных Нетологии.
1. Тесты могут не покрывать всех возможных негативных сценариев - всегда есть возможность, что пользователь поведет себя так, как мы не можем предвидеть. Эти риски придется закрывать уже не этапе продакшна.

# Перечень необходимых специалистов для автоматизации:

QA инженер с опытом автоматизации, умеющий работать с вышеперечисленными инструментами тестирования

# Интервальная оценка с учётом рисков (в часах):

С учетом необходимости оформления сопутствующей документации (тест-планы, баг-репорты, отчеты о тестировании), а также с поправкай на обстоятельства, которые могут повлиять на продолжительность тестирования (технические неисправности сервера, отсутствие необходимых разрешений, внесение изменений в инструментарий и тп.) интервальная оценка составляет около 20 часов.




