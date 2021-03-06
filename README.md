# Примеры UI автотестов для Android приложения Wikipedia (build 2.7.50391-alpha-2022-01-20)

## Cписок автоматизированных тест-кейсов в данном проекте:

- [x] Переключение между экранами Getting Started и проверка, что переход выполнен  
- [x] Добавление русского языка и проверка его наличия в списке
- [x] Выключение передачи анонимных данных о пользователе приложения и проверка, что передача выключена 

## Стек технологий:

![Intelij_IDEA](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Intelij_IDEA.png)![Java](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Java.png)![Selenide](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Selenide.png)![Selenoid](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Selenoid.png)![Gradle](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Gradle.png)![JUnit5](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/JUnit5.png)![Allure Report](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Allure_Report.png)![AllureTestOps](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/AllureTestOps.png)![Github](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Github.png)![Jenkins](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Jenkins.png)![Appium](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Appium.png)![Browserstack](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Browserstack.png)![Rest-Assured](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Rest-Assured.png)![Telegram](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Telegram.png)![Jira](https://github.com/andreigkuznetsov/smallUIproject/blob/master/img/icons/Jira.png)

Java, Gradle, JUnit5, Selenide, Jenkins, Selenoid, Allure Reports, TestOps, Appium, Browserstack, RestAssured, Telegram (уведомления), Jira

## Запуск тестов с заполненными конфигурационными файлами *.properties 
### (ниже показаны команды для запуска в Jenkins, для локального запуска в начало команды добавляем gradle):

### Для запуска тестов в BrowserStack:

```bash
clean test -DdeviceHost=browserstack
```
### Для запуска тестов в Selenoid:

```bash
clean test -DdeviceHost=selenoid
```
### Для запуска тестов в эмуляторе + Appium:

```bash
clean test -DdeviceHost=emulation
``` 
### Для запуска тестов на реальном устройстве + Appium:

```bash
clean test -DdeviceHost=real
``` 

### Для запусков автотестов используется Jenkins.

##### Примеры готовых сборок можно посмотреть [по ссылке](https://jenkins.autotests.cloud/job/09-andreikuzn-mobile-tests/)

### Анализ результатов запусков в Jenkins через Allure Reports

![Jenkins_Allure_Reports](img/allure_dashbord_mt.png)

![Jenkins_Allure_Reports1](img/allure_detailes_mt.png)

![Jenkins_Allure_Reports2](img/allure_detailes1_mt.png)

### Для отображения результатов сборок также используется Allure TestOps.

##### Примеры запусков и их результаты можно посмотреть [по ссылке](https://allure.autotests.cloud/project/920/dashboards)

### Пример списка тестов и их прохождения в Allure TestOps

![Allure TestOps](img/testops_detailes1_mt.png)

### Результаты запусков Launches в Allure TestOps

![Allure_Launches](img/testops_detailes_mt.png)

### Основной Dashboards

![Allure Dashboards](img/testops_dashbord_mt.png)

### Добавлена интеграция с Jira, где можно посмотреть запускаемые кейсы и их результаты.

##### Перейти в задачу Jira можно [по ссылке](https://jira.autotests.cloud/browse/HOMEWORK-312)

![Jira](img/Jira_mt.png)

### После прохождения тестов в telegram канал приходит оповещение с результами.

![Telegram](img/Telegram_mt.jpg)

### Пример прохождения тестов можно посмотреть на видео

![video](img/video_mt.gif)
