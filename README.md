# NetologyWebsiteTest
## План автоматизации
#### тестирования сценария перехода к форме записи на обучение профессии "Тестировщик ПО" и заполнения этой формы
### 1.	Перечень автоматизируемых сценариев
### Сценарии навигации

#### Сценарий 1.
1.	Открыть сайт https://netology.ru/
2.	Открыть меню «Каталог курсов» в шапке страницы
3.	Навести курсор мыши на раздел «Программирование»
4.	Выбрать курс «Тестировщик ПО»
5.	На открывшейся странице нажать на кнопку «Записаться»

#### Сценарий 2.
1.	Открыть сайт https://netology.ru/
2.	Открыть меню «Каталог курсов» в шапке страницы
3.	Выбрать раздел «Программирование»
4.	На открывшейся страницу выбрать курс «Тестировщик ПО»
5.	На открывшейся странице найти форму для записи

#### Сценарий 3.
1.	Открыть сайт https://netology.ru/
2.	Выбрать виджет «Нео для начинающих»
3.	На открывшейся страницу выбрать курс «Тестировщик ПО»
4.	На открывшейся странице нажать на кнопку «Записаться»

#### Сценарий 4.
1.	Открыть сайт https://netology.ru/
2.	Внизу страницы найти ссылку «Каталог курсов», перейти по ней.
3.	На открывшейся странице в правом фильтре в разделе «Направление» отметить «Программирование»
4.	На той же странице в правом фильтре в разделе «Уровень» отметить «Нео»
5.	Выбрать курс «Тестировщик ПО»
6.	На открывшейся странице найти форму для записи

#### Сценарий 5.
1.	Открыть сайт https://netology.ru/
2.	Открыть меню «Каталог курсов» в шапке страницы
3.	Выбрать раздел «Полный каталог»
4.	На открывшейся странице в правом фильтре в разделе «Направление» отметить «Программирование»
5.	Выбрать курс «Тестировщик ПО»
6.	На открывшейся странице найти форму для записи

### Сценарии тестирования

#### Сценарий 1. Ввод во все поля валидных данных

***Входные данные:***

* Имя – распространенное в России имя на кириллице
* Телефон – 11 цифр, начиная с +7
* Электронная почта – комбинация латинских букв, имеющая признаки электронной почты, например: test@host.com

***Шаги выполнения***
1.	В поле «Имя» ввести тестовое имя.
2.	В поле «Телефон» ввести тестовый номер телефона.
3.	В поле «Электронная почта» ввести тестовую электронную почту.
4.	Нажать кнопку «Записаться».

***Ожидаемый результат:***
Осуществляется переход на страницу подтверждения.

#### Сценарий 2. Отправка пустого значения поля "Имя"

***Входные данные:***

* Имя - пустое поле
* Телефон - 11 цифр, начиная с +7
* Электронная почта – комбинация латинских букв, имеющая признаки электронной почты, например: test@host.com 

***Шаги выполнения***
1.  Поле "Имя"	не заполнять
2.	В поле «Телефон» ввести тестовый номер телефона.
3.	В поле «Электронная почта» ввести тестовую электронную почту.
4.  Нажать кнопку «Записаться».

***Ожидаемый результат:***
У поля "Имя" появляется подсказка: «Поле обязательное для заполнения».

#### Сценарий 3. Отправка пустого значения поля "Телефон"

***Входные данные:***

* Имя – распространенное в России имя на кириллице
* Телефон - пустое поле
* Электронная почта – комбинация латинских букв, имеющая признаки электронной почты, например: test@host.com 

***Шаги выполнения***
1.	В поле «Имя» ввести тестовое имя.
2.	Поле «Телефон» не заполнять.
3.	В поле «Электронная почта» ввести тестовую электронную почту.
4.  Нажать кнопку «Записаться».

***Ожидаемый результат:***
У поля "Телефон" появляется подсказка: «Поле обязательное для заполнения».

#### Сценарий 4. Отправка пустого значения поля "Электронная почта"

***Входные данные:***

* Имя – распространенное в России имя на кириллице
* Телефон - 11 цифр, начиная с +7
* Электронная почта – пустое поле 

***Шаги выполнения***
1.	В поле «Имя» ввести тестовое имя.
2.	В поле «Телефон» ввести тестовый номер телефона.
3.	Поле «Электронная почта» не заполнять.
4.  Нажать кнопку «Записаться».

***Ожидаемый результат:***
У поля "Электронная почта" появляется подсказка: «Поле обязательное для заполнения».

#### Сценарий 5. Проверка поля «Имя» на раскладку

***Входные данные:***

* Имя – имя на латинице
* Телефон – 11 цифр, начиная с +7
* Электронная почта – комбинация латинских букв, имеющая признаки электронной почты, например: test@host.com 

***Шаги выполнения***
1.	В поле «Имя» ввести тестовое имя.
2.	В поле «Телефон» ввести тестовый номер телефона.
3.	В поле «Электронная почта» ввести тестовую электронную почту.

***Ожидаемый результат:***
У поля «Имя» появляется подсказка: «Используйте кириллицу».

#### Сценарий 6. Проверка поля «Телефон» на количество знаков меньше 11 цифр

***Входные данные:***

* Имя – распространенное в России имя на кириллице
* Телефон – 10 цифр, начиная с +7
* Электронная почта – комбинация латинских букв, имеющая признаки электронной почты, например: test@host.com

***Шаги выполнения***
1.	В поле «Имя» ввести тестовое имя.
2.	В поле «Телефон» ввести тестовый номер телефона.
3.	В поле «Электронная почта» ввести тестовую электронную почту.

***Ожидаемый результат:***
У поля «Телефон» появляется подсказка: «Номер телефона должен быть вида +70123456789».

#### Сценарий 7. Проверка поля «Электронная почта» на ввод символов без признаков электронной почты

***Входные данные:***

* Имя – распространенное в России имя на кириллице
* Телефон – 11 цифр, начиная с +7
* Электронная почта – комбинация латинских букв, не имеющая признаков электронной почты (@ и .)

***Шаги выполнения***
1.	В поле «Имя» ввести тестовое имя.
2.	В поле «Телефон» ввести тестовый номер телефона.
3.	В поле «Электронная почта» ввести тестовую электронную почту.

***Ожидаемый результат:***
У поля «Электронная почта» появляется подсказка: «Неверный email».

### 2.	Перечень используемых инструментов с обоснованием выбора

*	Git и GitHub — хранение кода, в том числе авто-тестов;
*	JUnitJupiter— платформа для написания авто-тестов и их запуска;
*	Java 11 — язык написания авто-тестов;
*	Gradle — система управления зависимостями
*	Faker – для генерации тестовых данных
*	REST-assured – для тестирования API
*	Selenide – для тестирования GUI
*	паттерн Page Object – для более гибкого взаимодействия с SUT и сокрытия внутреннего устройства определённой страницы или её виджетов за логическим интерфейсом взаимодействия
*	Allure – для формирования отчета о тестировании
### 3.	Перечень необходимых разрешений/данных/доступов
* Разрешения: На автотестирование сайта, на запись в БД, на чтение, на удаление.
* Данные: Тестовые Имя, Телефон, Электронная почта.
* Доступ: Доступ к базе данных для записи, для проверки, что внесенные данные занесены в БД, для удаления тестовых данных.
### 4.	Перечень и описание возможных рисков при автоматизации
*	Отсутствие CSS селекторов для тестирования.
*	Изменения страниц без уведомления тестировщиков
*	Получения доступа к БД может привести к внесению некорректных записей
*	Низкая скорость интернета или его отсутствие в момент тестирования
### 5.	Перечень необходимых специалистов для автоматизации
* Тестировщик-автоматизатор  
  Или
* Ручной тестировщик и
  Разработчик
### 6.	Интервальная оценка с учётом рисков (в часах)
16
