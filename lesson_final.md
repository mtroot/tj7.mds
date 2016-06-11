## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfjBtOHl2WXdKWEo5R0NkcENQdGt6b1d5VjFQYTFBVHU4VVhYY0dwbjZXc1U">Материалы заключительного занятия</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSG5jeEVCTzZPbmc">Refactoring & Fix</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFektNeHlid1F6eXc">0-refactoring-fix.patch</a>**
  - Добавились поля <a href="http://info.javarush.ru/translation/2014/10/06/Зачем-использовать-SerialVersionUID-внутри-Serializable-класса-в-Java.html">serialVersionUID</a>
  - Рефакторинг REST контроллеров и обработка ошибок по `@ControllerAdvice(annotations = RestController.class)`
  - Правка UTF-8 в редактировании профиля и регистрации (порядок `encodingFilter` и `springSecurityFilterChain` фильтров)
  - Удалился `contentType` для get в тестах REST контроллеров (`contentType` нужен только для `@RequestMapping(consumes=..`)
  - Добавилась авторизация в `RootControllerTest`

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Разбор домашнего задания HW10

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFaDN2V1g0bG9EaFE">HW10</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZi1KT2IwT1RxaFU">1-validation-exception.patch</a>**

>  Добавилась локализация `duplicate_email`

>  Обработка валидации формы для Ajax контроллеров сделана через `org.springframework.validation.BindException`

###  ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFYms4YUxEMHdxZHM">HW10 Optional: change locale</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFWU1tdmxsbS1lZjQ">2-change-locale.patch</a>**

>  еще вариант смены локали в lang.jsp вместо javascript: `href=${requestScope['javax.servlet.forward.request_uri']}?lang=..`

- <a href="http://forum.spring.io/forum/spring-projects/web/1077-differences-between-spring-message-and-fmt-message">spring-message vs fmt-message</a>
- <a href="http://pro-cod.ru/navbar-uroki-bootstrap-3.html">Bootstrap Navbar</a>

## Заключительное занятие

##  ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png)  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZkpVM19QWFBOQ2c">Деплой приложения в Heroku.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFcEtNQXBFeWJvVkk">3-heroku.patch</a>**

> В `DataJpaUserRepositoryImpl` добавилась защита от удаления-модификации Admin/User

-  <a href="http://habrahabr.ru/post/265591/">Деплой Java Spring приложения в PaaS-платформу Heroku</a>
```
Config Vars
  ERROR_PAGE_URL=...
  TOPJAVA_ROOT=/app

Datasources advanced
  ssl=true
  sslfactory=org.postgresql.ssl.NonValidatingFactory
```
-  Ресурсы:
   -  <a href="https://www.heroku.com/">PaaS-платформа Heroku</a></h3>
   -  Конфигурирование приложения для запуска через <a href="https://devcenter.heroku.com/articles/java-webapp-runner">Tomcat-based Java Web</a>
   -  Конфигурирование <a href="https://devcenter.heroku.com/articles/connecting-to-relational-databases-on-heroku-with-java#using-the-database_url-in-spring-with-xml-configuration">DataSource profile для Heroku</a>
   -  <a href="http://www.jetbrains.com/idea/webhelp/run-debug-configuration-heroku-deployment.html">Интерграция с IDEA</a>
   -  <a href="http://www.paasify.it/filter">Find your Platform as a Service</a>
   -  <a href="https://devcenter.heroku.com/articles/getting-started-with-java#set-up">Getting Started with Java on Heroku</a>
   -  <a href="https://devcenter.heroku.com/articles/keys">Managing Your SSH Keys</a>
   -  <a href="https://devcenter.heroku.com/articles/getting-started-with-spring-mvc-hibernate#deploy-your-application-to-heroku">Deploy your application to Heroku</a>
   -  <a href="http://www.ibm.com/developerworks/ru/library/j-javadev2-21/">Развертывание приложений Java с помощью PaaS от Heroku</a>
   -  <a href="http://www.infoq.com/articles/paas_comparison">A Java Developer’s Guide to PaaS</a>
   -  <a href="https://dzone.com/articles/simple-paas-comparison-guide">A Simple PaaS Comparison Guide (With the Java Dev in Mind)</a>
   -  <a href="http://www.ibm.com/developerworks/library/j-paasshootout/">Java PaaS shootout</a>

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Домашнее задание по проекту:

    Код для деплоя в Heroku был включен в проект, из за чего некоторые тесты перестали проходить.
    Найти этот код и проверить что без него все работает.
    
    Сделать / обновить резюме
    Отдать на ревью мне или группе
    Заполнить форму "разработчик Java"

- <a href="https://github.com/JavaOPs/topjava/blob/master/cv.md">Составление резюме, подготовка к интервью, поиск работы</a>
- <a href="http://goo.gl/forms/Oy5A7HNkWt">Форма соискателя "Разработчик Java"</a>.

## Возможные доработки приложения:
-  Перевести UI на <a href="http://angular.ru/">angular.js</a> / <a href="https://vaadin.com/elements">Vaadin elements</a> /GWT /GXT /Vaadin / ZK/ [Ваш любимый фреймворк]..
-  Перевести проект на <a href="http://projects.spring.io/spring-boot/">Spring Boot</a>
-  Перевести шаблоны с JSP на <a href="http://www.thymeleaf.org/doc/articles/petclinic.html">Thymeleaf</a>
-  Для редактирования паролей сделать отдельный интерфейс с запросом старого пароля и кнопку сброса пароля для администратора.
-  Сделать авторизацию в приложение по OAuth 2.0 (<a href="http://projects.spring.io/spring-security-oauth/">Spring Security OAuth</a>,
<a href="https://vk.com/dev/auth_mobile">VK auth</a>, <a href="https://developer.github.com/v3/oauth/">github oauth</a>, ...)
-  Сделать подтверждение регистрации пользователя по email c возможностью восстановления пароля.
-  Интергировать проект с <a href="https://stormpath.com/">Identity API</a> <a href="https://docs.stormpath.com/java/spring-boot-web/quickstart.html">Stormpath</a>
-  Сделать отображение еды постранично, с поиском и сортировкой на стороне сервера.
-  Перевод проекта на https
-  Сделать desktop/mobile приложение, работающее по REST с нашим приложением.
-  Локализация сообщений об ошибках, показ ошибок в форме редактирования таблицы в стиле JSP.
-  <a href="http://www.mkyong.com/spring-security/spring-security-limit-login-attempts-example">Limit login attempts example</a>
-  Любая на ваше усмотрение.

**Если у Вас появилось желание доработать приложение и распространить код для других участников-
связывайтесь со мной для ревью и его оформления.**

## <a href="https://drive.google.com/folderview?id=0B9Ye2auQ_NsFflp6ZHBLSFI2OGVEZ2NQU0pzZkx4SnFmOWlzX0lzcDFjSi1SRk5OdzBYYkU">Все материалы проекта</a>

### Ресурсы по Проекту
-  <a href="https://chrome.google.com/webstore/detail/markdown-preview/jmchmkecamhbiokiopfpnfgbidieafmd?utm_source=chrome-app-launcher-info-dialog">Плагин Markdown Preview для Хрома</a>
-  <a href="http://pro-cod.ru/uroki-bootstrap-3-0">Уроки Bootstrap 3</a>
-  <a herf="http://www.tutorialspoint.com/spring/index.htm">Spring at tutorialspoint</a>
-  <a href="http://www.codejava.net/frameworks/spring">Articles in Spring</a>
-  <a href="http://www.baeldung.com/learn-spring">Learn Spring on Baeldung</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/index.html">Spring Framework
            Reference Documentation</a>
-  <a href="http://docs.jboss.org/hibernate/orm/4.3/manual/en-US/html/">Hibernate Reference Documentation</a>
-  <a href="http://java-course.ru/student/book2/">Java Course (книга 2)</a>
-  <a href="http://design-pattern.ru/">Справочник «Паттерны проектирования»</a>
-  <a href="http://martinfowler.com/eaaCatalog/">Catalog of Patterns of Enterprise Application Architecture</a>

# ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) <a href="http://goo.gl/forms/PtFcPqEV5n">Короткий опрос для всех участников проекта</a>

### Приглашаю всех в <a href="https://join.skype.com/dToijYHZNcuc">группу выпускников 'Online Projects' в skype</a> (перед добавлением залогинтесь в аккаунт skype).
Это общение по теме java, трудоустройство, зарплаты и пр. Добавиться можно по ссылке или напиши мне в скайп и я добавлю.
