# План тестирования накопительного счета "Накопилка"
## Перечень автоматизированных сценариев:
Позитивные сценарии:
Проверить возможность входа в "Накопилку" через вкладку "Частным лицам" и через "Вклады"
1. Открываем сайт 
2. Переходим во вкладку Частным лицам/Вклады
3. Переходим в накопилку

Ождаемый результат: открывается сайт с накопилкой

Заполнение заявки с валидным именем и валидным мобильным телефоном
1. Переходим в Накопилку. 
2. Жмем кнопку "заполнить заявку"
3. Заполняем поля валидными данными (правила заполнения должен предоставить сам банк), жмем галочку с соглашением
4. Отправляем

Ожидаемый результат: сообщение с принятием заявки

Исключить возможность отправки заявки без согласия на обработку персональных данных
1. Переходим в Накопилку. 
2. Жмем кнопку "заполнить заявку"
3. Заполняем поля валидными данными (правила заполнения должен предоставить сам банк), но не жмем на галочку с соглашением
4. Отправляем

Ожидаемый результат: возникновение ошибки, форма не отправляется

Негативные сценарии:

Заполнение заявки с невалидными данными телефона
1. Переходим в Накопилку. 
2. Жмем кнопку "заполнить заявку"
3. Заполняем поля невалидными данными телефона (правила заполнения должен предоставить сам банк), жмем на галочку с соглашением
4. Отправляем 

Ожидаемый результат: возникновение ошибки, форма не отправляется

Заполнение заявки с невалидными данными имени
1. Переходим в Накопилку. 
2. Жмем кнопку "заполнить заявку"
3. Заполняем поля невалидными данными имени (правила заполнения должен предоставить сам банк), жмем на галочку с соглашением
4. Отправляем 

Ожидаемый результат: возникновение ошибки, форма не отправляется

## Перечень используемых инструментов:
1. Java 11 - один из лидирующих языков на рынке. Его часто используют для тестирования, так как он имеет постоянно обновляющиеся удобные фреймворки для тестирования, например, JUnit. 
2. Junit5 - имеет новое строение по сравнению с предыдщуими JUnit. Содержит в себе Junit Platform + JUnit Jupiter + Junit Vintage. Если говорить коротко у данного фреймворка приоритет как минимум из-за удобства и быстроты работы с ним
3. IntellyJ IDEA - одна из самых популярных сред разработки на java. Может исправлять автоматически ошибки, всегда всплывают подсказки и предупреждения. Удобство использования.
4. Gradle - система сборок. Онf контролирует процесс разработки в задачах от компиляции и упаковки до тестирования, развертывания и публикации. Очень много поддерживаемых языков, включая Java, JavaScript и др.
5. Allure - система отчетности по тестированию. Наглядный и удобный фреймворк. Прост для работы.
6. MySQL - СУБД, одна из распространненых. Удобна и практична
7. Postman - используется для тестирования API и нагрузки сервисов

## Перечень необходимых разрешений/данных/доступов от банка:
1. Разрешение соответственно на само тестирование
2. Доступ к некоторым действующим аккаунтам для того, чтобы убедиться, что зарегистрированным пользователям нужно точно также проходить анкету для "Накопилки"
3. Правила заполнения данных в форме для отправки "Накопилки" (минимальные,максимальные размеры полей, доступно ли использование символов, латинских букв, можно ли писать имя разного регистра, сколько цифр разрешено для ввода номера, с какой цифры или знака должен начинаться номер)
4. Доступ к БД и API 

## Перечень и описание возможных рисков при автоматизации
1. Возможное падение сайта во время нагрузочного тестирования
2. Изменение структуры сайта, вследствие чего тесты придется снова изменять

## Перечень необходимых специалистов для автоматизации
QA-инженер с опытом работы в автоматизации

## Интервальная оценка без учёта риска и с учётом рисков (в часах)
1. Без учёта - 8 часов
2. С учётом - 9,5-10 часов
