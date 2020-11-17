# План тестирования накопительного счета "Накопилка"
## Перечень автоматизированных сценариев:
Позитивные сценарии:
1. Проверить возможность входа в "Накопилку" через вкладку "Частным лицам" и через "Вклады"
  1.1. Открываем сайт 
  1.2. Переходим во вкладку Частным лицам/Вклады
  1.3. Переходим в накопилку
Ождаемый результат: открывается сайт с накопилкой

2. Заполнение заявки с валидным именем и валидным мобильным телефоном
###2.1. Переходим в Накопилку. 
###2.2. Жмем кнопку "заполнить заявку"
###2.3. Заполняем поля валидными данными (правила заполнения должен предоставить сам банк), жмем галочку с соглашением
###2.4. Отправляем
Ожидаемый результат: сообщение с принятием заявки

3. Исключить возможность отправки заявки без согласия на обработку персональных данных
###3.1. Переходим в Накопилку. 
###3.2. Жмем кнопку "заполнить заявку"
###3.3. Заполняем поля валидными данными (правила заполнения должен предоставить сам банк), но не жмем на галочку с соглашением
###3.4. Отправляем 
Ожидаемый результат: возникновение ошибки, форма не отправляется

Негативные сценарии:

1. Заполнение заявки с невалидными данными телефона
###1.1. Переходим в Накопилку. 
###1.2. Жмем кнопку "заполнить заявку"
###1.3. Заполняем поля невалидными данными телефона (правила заполнения должен предоставить сам банк), жмем на галочку с соглашением
###1.4. Отправляем 
Ожидаемый результат: возникновение ошибки, форма не отправляется
2. Заполнение заявки с невалидными данными имени
###2.1. Переходим в Накопилку. 
###3.2. Жмем кнопку "заполнить заявку"
###4.3. Заполняем поля невалидными данными имени (правила заполнения должен предоставить сам банк), жмем на галочку с соглашением
###4.4. Отправляем 
Ожидаемый результат: возникновение ошибки, форма не отправляется

## Перечень используемых инструментов:
1. Java 11 - один из лидирующих языков на рынке. Его часто используют для тестирования, так как он имеет постоянно обновляющиеся удобные фреймворки для тестирования, например, JUnit. 
2. Junit5 - имеет новое строение по сравнению с предыдщуими JUnit. Содержит в себе Junit Platform + JUnit Jupiter + Junit Vintage. Если говорить коротко у данного фреймворка приоритет как минимум из-за удобства и быстроты работы с ним
3. IntellyJ IDEA - одна из самых популярных сред разработки на java. Может исправлять автоматически ошибки, всегда всплывают подсказки и предупреждения. Удобство использования.

## Перечень необходимых разрешений/данных/доступов от банка:
1. Разрешение соответственно на само тестирование
2. Доступ к некоторым действующим аккаунтам для того, чтобы убедиться, что зарегистрированным пользователям нужно точно также проходить анкету для "Накопилки"
3. Правила заполнения данных в форме для отправки "Накопилки" (минимальные,максимальные размеры полей, доступно ли использование символов, латинских букв, можно ли писать имя разного регистра, сколько цифр разрешено для ввода номера, с какой цифры или знака должен начинаться номер)

## Перечень и описание возможных рисков при автоматизации
1. Времязатратно. Возможно, ручное тестирование было бы здесь полезнее и быстрее
2. Денежнозатратно. Ручное тестирование вышло бы куда дешевле

## Перечень необходимых специалистов для автоматизации
QA-инженер с опытом работы в автоматизации

## Интервальная оценка с учётом рисков (в часах)
От 8 до 10 часов, включая повторные проверки
