# Онлайн проекта <a href="https://github.com/JavaWebinar/topjava07">Topjava</a>

- **<a href="https://github.com/JavaOPs/topjava/wiki/Git">Напоминаю про работу с патчами (GIT Wiki)</a>**

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfm5hSHEtbmxmN2kxb0NocVRwWl9KanowWXVCVXRZTlhaM09wQUswZkRidTA">Материалы 1-го урока</a>

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Разбор домашнего задания HW0:
### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFOGU0a3ZUbFo3Skk">Optional: реализация getFilteredMealsWithExceeded через Stream API</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFS1FZak55T0Y4cEU">1-1-HW0-stream.patch</a>**

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFdTJIQUExajZWWkE">Работа с git в IDEA. Реализация через цикл.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSWxmSExhR0xydU0">1-2-HW0-cycle.patch</a>**

> Изменения в проекте: `map.getOrDefault` земенил на `map.merge`, `for` заменены на `forEach`

## Занятие 1:
### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 3. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFRmo0YkVVaDJPTVE">Обзор используемых в проекте технологий. Интеграция ПО.</a>
-  <a href="http://zeroturnaround.com/rebellabs/java-tools-and-technologies-landscape-for-2014/">Обзор популярности инструментов и технологий Java за 2014 г.</a>
-  <a href="http://www.youtube.com/watch?v=rJZHerwi8R0">Видео "Приложение Spring Pet Clinic"</a> 
-  Приложение <a href="https://github.com/spring-projects/spring-petclinic">Spring Pet Clinic</a>. 
-  Demo <a href="http://petclinic.cloudapp.net/">Spring Pet Clinic</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 4. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSlZMTXBJRXJpakU">Maven.</a>
- Среда сборки проектов <a href="http://www.apache-maven.ru/" target="_blank">Maven</a>.
- <a href="http://search.maven.org/#browse">The Central Repository</a>
- Настройка пропертей Maven: кодировка, java version, зависимости, maven-compiler-plugin
- <a href="http://maven.apache.org/guides/mini/guide-multiple-modules.html">The Reactor</a>. Snapshots
- <a href="http://habrahabr.ru/blogs/java/106717/" target="_blank">Недостатки Maven</a>. Другие инструменты сборки.
- Справочник:
  - <a href="http://habrahabr.ru/post/77333/">Автоматизация сборки проекта</a>
  - <a href="http://maven.apache.org/">Home Page</a>
  - <a href="http://books.sonatype.com/mvnref-book/reference/index.html">Maven: The Complete Reference</a>
  - <a href="http://study-and-dev.com/blog/build_management_maven_1/">Разработка ПО вместе с maven</a>
  - <a href="http://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html">Build Lifecycle</a>
  - <a href="http://maven.apache.org/guides/introduction/introduction-to-dependency-mechanism.html">Dependency Mechanism</a>
  - <a href="http://habrahabr.ru/post/111408/">Создание своих архетипов и каталогов в Maven</a>
  - <a href="http://www.ibm.com/developerworks/ru/library/j-5things13/">Зависимости, профили</a>
  - <a href="http://blog.bintray.com/2014/02/11/bintray-as-pain-free-gateway-to-maven-central/">Bintray: gateway to Maven Central</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 5. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFT3pWNkMzWVVybnc">WAR. Веб-контейнер Tomcat. Сервлеты.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSlRSZVlYeHpJbUE">1-3-switch-to-war.patch</a>**
> Сервлет добавляется в следующем патче, те в web.xml он будет подчеркиваться красным.

- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVWVGZ1FIUkFHYXM">1-4-add-servlet-api.patch</a>**
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFMXlZN0tGSjJRZW8">1-5-forward-to-redirect.patch</a>**
- Перевод проекта на Web.
- <a href="http://tomcat.apache.org/">Tomcat Home Page</a>
- <a href="http://java-course.ru/student/book1/servlet/">Сервлеты.</a>
- Настройка и деплой в Tomcat. Tomcat manager. Remote debug.
- Запуск Tomcat из IDEA. Динамическое обновление без передеплоя.
- Redirect, Forward, Application context, Servlet context
    - Томкат менеджер: <a href="http://localhost:8080/manager">http://localhost:8080/manager</a>
    - Наше приложение: <a href="http://localhost:8080/topjava">http://localhost:8080/topjava</a>
    - Наш сервлет:     <a href="http://localhost:8080/topjava/users">http://localhost:8080/topjava/users</a>
- Справочник:
  - <a href="http://info.javarush.ru/idea_help/2014/01/22/Руководство-пользователя-IntelliJ-IDEA-Отладчик-.html">Отладчик IntelliJ IDEA</a>
  - <a href="https://www.youtube.com/watch?v=tN8K1y-HSws&list=PLkKunJj_bZefB1_hhS68092rbF4HFtKjW&index=14">Yakov Fain: Intro to Java EE. Glassfish. Servlets (по русски)</a>
  - <a href="https://www.youtube.com/watch?v=Vumy_fbo-Qs&list=PLkKunJj_bZefB1_hhS68092rbF4HFtKjW&index=15">Yakov Fain: HTTP Sessions, Cookies, WAR deployments, JSP (по русски)</a>
  - <a href="https://www.youtube.com/playlist?list=PLoij6udfBncjHaO5s7Ln4w4BLj5FVc49P">Golovach Courses: Junior.February2014.Servlets</a>
  - <a href="http://blog.trifork.com/2014/07/14/how-to-remotely-debug-application-running-on-tomcat-from-within-intellij-idea">Remotely debug on tomcat from IDEA</a>
  - <a href="http://www.java2ee.ru/jsp/">Java Server Page</a>
  - <a href="http://java-online.ru/jsp.xhtml">Java Server Pages (JSP)</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 6. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFaTdYUnpLNFFUeXM">Логирование.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTEZfcXBHT0k5eGM">1-6-logging.patch</a>**
> **установите переменную окружения на TOPJAVA_ROOT на корень проекта и перезапустите IDEA**

> изменения в проекте: убрал `LoggerWrapper` и логирую напрямую в логгер SLF4J. При логгировании через вспомогательный класс, в логе теряется имя исходного класса.

- <a href="http://habrahabr.ru/post/113145/">Java Logging: история кошмара</a>
- <a href="http://skipy.ru/useful/logging.html">Ведение лога приложения</a>
- <a href="http://logging.apache.org/log4j/2.x/index.html">Log4j</a>, <a href="http://logback.qos.ch/">Logback</a>
- <a href="http://www.slf4j.org/legacy.html">Добавление зависимостей логирования</a> в проект. Переменная окружения TOPJAVA_ROOT
- Конфигурирование логирования. Настройка Live Template.
- Тестирование логирования в сервлете.

#### Проверочные вопросы:
- Что нужно изменить в `pom.xml`, чтобы перейти с logback на log4j ?

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 7. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFeE9LQTdDOTZTOGc">Подсоединение к логгеру по JMX. Выбор работы.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNjVocFBQSU94enc">1-7-remote-jmx.patch</a>**

> Для подключения к Remote Process (`localhost:1099`) положить `setenv.bat` в `$TOMCET_HOME/bin`.

- Управление логированием по <a href="https://ru.wikipedia.org/wiki/Java_Management_Extensions">Java Management Extensions</a>.

### ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) Ваши вопросы

>  Используются ли еще где-то в реальной разработке JSP, или это уже устаревшая технология? Заменит ли ее JSF (https://javatalks.ru/topics/38037)?

JSF и JSP- разные ниши и задачи.
JSP- шаблонизатор, JSF- МVС фреймворк. Из моего опыта- с JSP сталкивался в 60% проектов. Его прямая замена: http://www.thymeleaf.org, но пока встречется достаточно редко. JSP не умирает, потому что просто и дешево. Кроме того включается в большнство веб-контейнеров (в Tomcat его реализация Jasper)

JSF- sun-овский еще фреймворк, с которым я ни разу не сталкивался и особого желания нет. Вот он как раз, по моему мнению, активно замещается хотябы angular.


> А зачем мы использовали logback? Почему SLF4J нас не устроило? Почему реализация логирования не log4j?

`SLF4J-API` это API. Там есть только пустая реализация `org.slf4j.helpers.NOPLogger` (можно посмотреть в исходниках). Logback для новых проектов стал стандарт. spring-petclinic и spring-boot используют его.
- http://logback.qos.ch/reasonsToSwitch.html

---------

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Домашнее задание HW01 (делаем ветку HW01 от последнего патча)

- По аналогии с `UserServlet` добавить `MealServlet` и `mealList.jsp`.
  - Задеплоить приложение (war) в Tomcat c `applicationContext=topjava` (приложение должно быть доступно по <a href="http://localhost:8080/topjava">http://localhost:8080/topjava</a>)
  - Попробовать разные деплои в Tomcat, remote и local debug
- Сделать отображения списка еды в jsp, цвет записи в таблице зависит от параметра `isExceeded` (красный/зеленый).
  - Время выводить без 'T', список выводим БЕЗ фильтрации, `user` к `UserMeal` НЕ добавляем.
  - Вариант реализации:
    - из сервлета преобразуете еду в памяти в `List<UserMealWithExceeded>`;
    - кладете список в запрос (`request.setAttribute`);
    - делаете forward на jsp для отрисовки таблицы (при redirect аттрибуты теряются).
  - Деплоиться лучше как `war exploded`: нет упаковки в war и при нажатой кнопке `Update Resources on Frame Deactivation` можно обновляться css, html, jsp без передеплоя. При изменении `web.xml`, добавлении методов, классов необходим redeploy.
  - В `JSP` для цикла можно использовать `JSTL tag forEach`. Для подключения `JSTL` в `pom.xml` и шапку JSP нужно добавить:
```
    <dependency>
       <groupId>javax.servlet</groupId>
       <artifactId>jstl</artifactId>
       <version>1.2</version>
    </dependency>

    <%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
    ...
```

  - <a href="http://java-course.ru/student/book1/servlet/">Интернет-приложения на JAVA</a>
  - <a href="http://stackoverflow.com/questions/246859/http-1-0-vs-1-1">HTTP 1.0 vs 1.1</a>
  - <a href="http://java-course.ru/student/book1/jsp/">JSP</a>
  - <a href="http://devcolibri.com/1250">JSTL для написания JSP страниц</a>
  - <a href="http://javatutor.net/articles/jstl-patterns-for-developing-web-application-1">JSTL: Шаблоны для разработки веб-приложений в java</a>

#### Optional

- Сделать В ПАМЯТИ реализацию CRUD (create/read/update/delete) для еды с учетом многопоточности (хранение в памяти будет одна из наших реализаций, такжен будет JDBC, JPA и DATA-JPA)).
- В качестве ключа добавить `id` в `UserMeal/ UserMealWithExceed`.
- Работать с реализацией через интерфейс, который не должен ничего знать о деталях реализации (Map, DB или что-то еще).
- Сделать форму редактирования в JSP: AJAX/JavaScript использовать НЕ надо, делаем через `<form method="post">` и `doPost()` в сервлете.
- <a href="https://danielniko.wordpress.com/2012/04/17/simple-crud-using-jsp-servlet-and-mysql/">Simple CRUD using JSP, Servlet</a>

### ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Решение проблем

- Если вы не попадаете на страничку/брекпойнт в сервлете: 
  - внимательно проверьте url и applicationContext (Application Context должен быть тот же, что и url приложения: <a href="https://github.com/JavaOPs/topjava/wiki/IDEA#%D0%94%D0%B5%D0%BF%D0%BB%D0%BE%D0%B9-war-%D0%B2-tomcat-application-context-%D0%B4%D0%BE%D0%BB%D0%B6%D0%B5%D0%BD-%D0%B1%D1%8B%D1%82%D1%8C-%D1%82%D0%BE%D1%82-%D0%B6%D0%B5-%D1%87%D1%82%D0%BE-%D0%B8-url-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F-%D0%B4%D0%B5%D0%BF%D0%BB%D0%BE%D0%B8%D1%82%D1%8C-%D0%BD%D0%B0%D0%B4%D0%BE-war-exploded">wiki IDEA</a>)
  - посомтрите в task manager: возможно у вас запущено несколько JVM и они мешают друг другу.
- Проблемы с кодировкой в POST. Возможное решение:
```
protected void doPost(HttpServletRequest request, ...) {
    request.setCharacterEncoding("UTF-8");
```
- После выставления переменной окружения IDEA нужно рестартовать. Проверить, видит ли java переменную окуржения можно так: `System.getenv("TOPJAVA_ROOT")`. Еще вариант: добавить `-DTOPJAVA_ROOT=...` в опции запуска приложения, тогда она доступна из java как `System.getProperty("TOPJAVA_ROOT")`.
----------------------------

### ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Типичные ошибки
- Хранить нужно `UserMeal` и конвертировать ее в `UserMealWithExceed` когда отдаем список на отображение в JSP. Иначе при редактировании любой записи или изменении юзером своей нормы `caloriesPerDay` нужно будет пересчитывать все записи юзера.
- Стили `color` можно применять ко всей строке таблицы `tr`, а не каждой ячейке.
- DateTimeFormatter можно сделать один заранее (он потокобезопасный в отличии от SimpleDateFormatter), а не создавать новый при каждом запросе.
- Реализаций интерфейса хранения будет несколько. Нужно учитывать это в названии класса.
- Если в названии класса есть Meal, не нужно использовать слово meal в методах класса.
