## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfkF5c1hiWmstT0prODdtZkVuNFlMZmdtN3J0OUcyY0lkT2NlVzlUMXRUUlk">Материалы 6-го урока</a>

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Разбор домашнего задания HW5

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUVZobXRzNWFzUW8">HW5: Spring Profiles. Spring Data JPA</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZk5Wc1ZuY2d5ZEk">01-HW5-data-jpa.patch</a>**
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFRVVWbHh3bjdBUTg">02-HW5-profiles.patch</a>**
> Для IDEA не забудте выставить Spring Profiles в `spring-db.xml`: нарпимер `datajpa, postgres`

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFbjAwQngzUWdjXzQ">3-HW5-tests.patch</a>**
> `DbTest` переименован в `AbstractServiceTest` и сюда перенесли `@ActiveProfiles(Profiles.POSTGRES)`

>  Т.к. HSQLDB не понимает LocalDateTime, разделил `JdbcUserMealRepositoryImpl` на `Java8JdbcUserMealRepositoryImpl` и `TimestampJdbcUserMealRepositoryImpl`
- <a href="https://www.javacodegeeks.com/2013/10/spring-4-conditional.html">Spring 4 Conditional</a>. Зайдите в исходники @Profile и посмотрите его  реализацию.

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFejhtNkI0RGpVd1E">HW5: Optional</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFajl3N2p0WEF1Z28">4-HW5-Optional-fix-servlet-main.patch</a>**
-  <a href="http://javarticles.com/2013/12/spring-profiles.html">Spring Profiles</a>
> Добавлены константы `Profiles.ACTIVE_DB`, `Profiles.DB_IMPLEMENTATION`

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFLVJ4LWcwQUhmLTA">5-HW5-Optional-fetch-join.patch</a>**
-  <a href="http://stackoverflow.com/questions/11938253/jpa-joincolumn-vs-mappedby">JPA JoinColumn vs mappedBy</a>
-  <a href="https://en.wikibooks.org/wiki/Java_Persistence/OneToMany#Unidirectional_OneToMany.2C_No_Inverse_ManyToOne.2C_No_Join_Table_.28JPA_2.x_ONLY.29">Unidirectional OneToMany</a>
> Добавлены проверки и тесты на `NotFound` для `UserMealService.getWithUser` и  `UserService.getWithMeals`


## Занятие 6:
### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFeTV0SUFfblk5NE0">Кэш Hibernate</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUlNzRXF6NHNubFk">6-hibernate-cache.patch</a>**
>  JdbcUserServiceTest поломася. Требуется починить в HW6

-  <a href="http://habrahabr.ru/post/135176/">Уровни кэширования Hibernate</a>
-  <a href="http://habrahabr.ru/post/136375/">Hibernate Cache. Практика</a>
-  <a href="http://www.tutorialspoint.com/hibernate/hibernate_caching.htm">Hibernate - Caching</a>
-  Починка тестов: <a href="http://stackoverflow.com/questions/1603846/hibernate-2nd-level-cache-invalidation-when-another-process-modifies-the-databas">инвалидация кэша Hibernate</a>
-  Ресурсы:
   -  Подключение <a href="http://www.ehcache.org/generated/2.9.0/html/ehc-all/#page/Ehcache_Documentation_Set%2Fco-hib_about_using_ehcache_with_hibernate.html%23wwconnect_header">кэша Hibernate 2-го уровня</a>
   -  <a href="http://stackoverflow.com/questions/3663979/how-to-use-jpa2s-cacheable-instead-of-hibernates-cache">JPA2 @Cacheable vs Hibernate @Cache</a>
   -  <a href="http://habrahabr.ru/post/25140/">Распределённая система кеша ehcache</a>
   -  <a href="http://docs.jboss.org/hibernate/orm/4.3/manual/en-US/html_single/#performance-cache-mapping">Cache mappings</a>
   -  <a href="http://vladmihalcea.com/2015/06/08/how-does-hibernate-query-cache-work/">How does Hibernate Query Cache work</a>
   -  <a href="http://blog.jhades.org/setup-and-gotchas-of-the-hibernate-second-level-and-query-caches/">Pitfalls of the Hibernate Second-Level / Query Caches</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2.  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVE1jWkRucm1UTjA">Spring Web</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFaTM4U0IzVlBnR00">7-spring-web.patch</a>**

-  Добавляем в проект веб зависимости
-  Поднятие контекста Spring в веб приложении. <a href="http://www.mkyong.com/servlet/what-is-listener-servletcontextlistener-example/">ServletContextListener</a>. Задание дефолтного профиля.
-  Получение контекста Spring в веб-контейнере
-  <a href="https://docs.oracle.com/javaee/6/tutorial/doc/bnafi.html">Servlet Lifecycle</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 3.   <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFN3k0ZVk1MnF5TjQ">JPS, JSTL, internationalization</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFeFY3SThJa0hHVFk">8-jsp-jstl-i18n.patch</a>**
-  <a href="http://www.java2ee.ru/jsp/include.html">jsp:include</a>
-  Имплементируем UserController. <a href="http://design-pattern.ru/patterns/mvc.html">Паттерн MVC</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 4.   <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFLTB3R3pKNFNEQmM">Динамическое изменение профиля при запуске.</a>
>  -Dspring.profiles.active="datajpa,postgres"

- <a href="http://stackoverflow.com/questions/10041410/default-profile-in-spring-3-1#answer-10041835">Set profiles in Spring 3.1</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 5.   <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFdkFRRFdYa0NoWkU">Конфигурирование Tomcat через maven plugin. Jndi-lookup.</a>
> `javax.el-api` scope изменил на `provided` (`el-api.jar` является частью Tomcat)

Запуск из коммандной строки (`clean` нужен для удаления из сборки зависимости `javax.el-api`):

     mvn clean org.apache.tomcat.maven:tomcat7-maven-plugin:run

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFb3pISVRYbGsxc1E">9-tomcat-pool-jndi.patch</a>**

- <a href="https://tomcat.apache.org/maven-plugin-2.0/tomcat7-maven-plugin/">Tomcat Maven Plugin</a>
- <a href="https://tomcat.apache.org/tomcat-7.0-doc/jndi-resources-howto.html"/>Tomcat JNDI Resources</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 6. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQThUX2VyQXNiTHM">Spring Web MVC</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVUxZQUktSWhJaU0">10-spring-webmvc.patch</a>**

-  <a class="anchor" id="mvc"></a><a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html">Spring Web MVC</a>
-  <a href="http://design-pattern.ru/patterns/front-controller.html">Паттерн Front Controller</a>
-  Добавляем DispatcherServlet и MVC application context.
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/integration-testing.html#testcontext-ctx-management-ctx-hierarchies">Иерархия контекстов в Spring Web MVC</a>
-  <a href="http://www.tutorialspoint.com/spring/spring_web_mvc_framework.htm">Сценарий обработки запроса</a>. <a href="http://www.studytrails.com/frameworks/spring/spring-mvc.jsp">HandlerMappings</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#mvc-viewresolver-resolver">View resolving</a>: прячем jsp под WEB-INF.
-  HandlerMapping: <a href="http://www.mkyong.com/spring-mvc/spring-mvc-simpleurlhandlermapping-example/">SimpleUrlHandlerMapping</a>, <a href="http://www.mkyong.com/spring-mvc/spring-mvc-beannameurlhandlermapping-example/">BeanNameUrlHandlerMapping</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#mvc-config-static-resources">Маппинг ресурсов.</a>
-  Ресурсы:
   -  <a href="http://www.jpalace.org/document/34/spring-mvc-tutorial">Spring MVC Tutorial</a>
   -  <a href="http://www.mkyong.com/spring-mvc/spring-mvc-hello-world-example/">Spring MVC hello world</a>
   -  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html">Web MVC framework</a>
   -  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#mvc-webappctx-special-beans-tbl">Special bean types in the WebApplicationContext</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 7. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUEctTkRSMWNvRjg">Spring Internationalization</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNFhpaTFUSkxScms">11-spring-i18n.patch</a>**

> Убедитесь что <a href="https://github.com/JavaOPs/topjava/wiki/IDEA#%D0%9F%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%B8%D1%82%D1%8C-%D0%BA%D0%BE%D0%B4%D0%B8%D1%80%D0%BE%D0%B2%D0%BA%D1%83-utf-8">в настройках IDEA кодировка везде UTF-8</a>

> Проверьте, что файлы локализации у вас в UTF-8 (в IDEA справа внизу в статусе есть кодировка и можно перекодировать).

-  <a href="http://simplespringtutorial.com/i18n.html">Spring Internationalization or i18n</a>
-  <a href="http://learningviacode.blogspot.ru/2012/07/reloadable-messagesources.html">Reloadable MessageSources</a>
-  <a href="http://nginx.com/resources/admin-guide/serving-static-content/">nginx: Serving Static Content</a>

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Домашнее задание HW06
    - Починить InMemory и Jdbc тесты

    - Добавить локализацию и jsp:include в meal*.jsp

    Починить работу meals: перенести функциональность MealServlet в контроллеры,
    разнести запросы на update/delete/.. по разным методам
    (можно делать по аналогии с ru.javawebinar.topjava.web.RootController#setUser,
    аннотации на параметры и адаптеры для LocalDate\Time мы введем позже).

Optional

    Добавить еще одну роль к админу (у него будет 2 роли: ROLE_USER, ROLE_ADMIN), 
                   добавить проверку ролей в тесты на User, починить тесты Jpa (дублирование)

    Починить тесты на роли Jdbc:
           добавить транзакционность (DataSourceTransactionManager) и доставание ролей в JdbcUserRepositoryImpl

## ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) Ваши вопросы
>  Кэш hibernate надстраивается над ehcache или он живет самостоятельно?

- <a href="http://mrbool.com/understanding-hibernate-caching/28721">Understanding Hibernate Caching</a>:
Hibernate supports following open-source cache implementations out-of-the-box: EHCache (Easy Hibernate Cache), OSCache (Open Symphony Cache), Swarm Cache, and JBoss Tree Cache.

> Где конфигурится интернализация для jstl? Т.е. файл, где здаются app, app_ru.properties. Достаточно указать в страницах бандл и путь в ресурсы?

`<fmt:setBundle basename="messages.app"/>` означает что ресурсы будут искаться в `classpath:messages\app(_xx)/properties`:
<a href="http://docs.oracle.com/javaee/5/jstl/1.1/docs/tlddocs/fmt/setBundle.html">Tag setBundle</a>: fully-qualified resource name, which has the same form as a fully-qualified class name.
После сборки проекта maven их можно найти в target\classes или target\topjava\WEB-INF\classes.


> Отлично, что она все пишет на том языке, который пришел в хидере запроса. А если я хочу выбрать?

Используется <a href="http://www.codejava.net/java-ee/jstl/jstl-format-tag-setlocale">JSTL Format Tag fmt:setLocale</a>. Мы переключимся на Spring i18n и переключение локалей будет реализовано в нем.

> Мы создаем бин, где получаем dataSource по имени `<jee:jndi-lookup id="dataSource" jndi-name="java:comp/env/jdbc/topjava"/>`.
Но там не указан класс, как в других dataSource? Получается по имени jdbc/topjava нам уже отдает готовый обьект dataSource и мы как бы помещаем его в бин?

Здесь используется namespace `jee:jndi-lookup`, который прячет под собой классы реализации. Сравните в http://habrahabr.ru/post/232381/ раздел Spring namespace configuration инициализацию базы через namespace jdbc и через классы.

> В плагине прописан профиль `<spring.profiles.active>tomcat,datajpa</spring.profiles.active>`, а в web.xml `<param-value>postgres,datajpa</param-value>`.
Какой же реально отрабатывает?

См видео урока "Динамическое изменение профиля при запуске". В плагине мы задаем параметры JVM запуска Tomcat

> Почему мы не используем элемент `<context:annotation-config/>` в `spring-db.xml`?

В проекте у нас сейчас 2 Spring контекста: `spring-mvc.xml (см. web.xml, DispatcherServlet)` и родительский `spring/spring-app.xml + spring/spring-db.xml (web.xml, contextConfigLocation)`.
Грубо: <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#d5e15231">2 мапы, причем для mvc доступно все что есть в родителе, но родитель не знает об mvc</a>. Те spring-db.xml не является отдельным самоcтоятельным контекстом и достаточно того, что `<context:annotation-config/>` у нас есть в `spring-app.xml`.

> В _ehcache.xml_ чем _<cache name="users"_ отличается от _<cache name="ru.javawebinar.topjava.model.User"_?

_user_ - это имя региона ecache, которое мы выбрали для кэширования c помощью Spring Cache `Collection<User> getAll()` в `UserServiceImpl`.
_ru.javawebinar.topjava.model.User_ - имя региона, которое использует Hibernate для кэширования содержимого таблицы _USERS_.
Мы можем оставить настройки по умолчанию, либо задать свои.

> A `@NamedQuery` или `@Query` подвержены кешу запросов? Т.е. если мы поставим _USE_QUERY_CACHE_value="true" будет Hibernate их кешировать?

Чтобы запрос кэшировался, кроме true в конфигурации нужно еще явно выставить запросу _setCacheable_ (http://vladmihalcea.com/2015/06/08/how-does-hibernate-query-cache-work/). По поводу кэширования @NamedQuery нашел _@QueryHint_: https://docs.jboss.org/jbossas/docs/Clustering_Guide/5/html/ch04s02s03.html

> Почему messages мы кладем в config и используем system environment? разве так делают в реальном проекте? не будешь же вписывать на сервере эти переменные каждый раз, если проект куда-то будет переезжать. Можно по другому, кроме systemEnvironment['TOPJAVA_ROOT'] задать путь от корня проекта?

1. messages нам нужны в runtime (при работе приложения). Проект к собранному и задеплоенному в Tomcat war отношения никакого уже не имеет и на этом сервере он обычно не находится. Если ресурсы нужны только при сборке и тестировании, то путь к корню для одномодульного maven проекта можно задать как ${project.basedir}, но для многомодульного проекта (а все реальные проекты многомодульные) это путь к корню своего модуля.
2. В "реальном приложении" делается совершенно по разному:
   - нести с собой в класспасе, но ресурсы нельзя будет динамически (без передеплоя) обновлять
   - класть в war (не в класспас) и обновлять в развернутом TOMCAT_HOME/webapps/[appname]/...
   - класть в зафиксированное определенное место (нарпимер в home: ~ или в путь от корня /app/congig). Можно задавать фиксированный пусть в пропертях профиля maven и фильтровать ресурсы (maven resources), чтобы они попали в проперти проекта.
   - делать через переменную окуржения, как у нас
   - задавать в параметрах запуска JVM как системную переменную через -D..
   - располагать в преференсах (для unix это home, для windows- registry): http://java-course.ru/articles/preferences-api/
   - держать настройки в DB

   Часто в одном приложении используют несколько способов для разных видов конфигураций.

---------------------
## ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Подсказки по HW06
- Неверная кодировка UTF-8 с Spring обычно решается фильтром `CharacterEncodingFilter`:
```
    <filter>
        <filter-name>encodingFilter</filter-name>
        <filter-class>org.springframework.web.filter.CharacterEncodingFilter</filter-class>
        <init-param>
            <param-name>encoding</param-name>
            <param-value>UTF-8</param-value>
        </init-param>
        <init-param>
            <param-name>forceEncoding</param-name>
            <param-value>true</param-value>
        </init-param>
    </filter>
    <filter-mapping>
        <filter-name>encodingFilter</filter-name>
        <url-pattern>/*</url-pattern>
    </filter-mapping>
```
- Функциональность еды в контроллерах должна быть в пакете meal и сделайте как для User - наследование от абстрактного класса.
- Если неправильно формируется url относительно контекста приложения посмотрите http://stackoverflow.com/questions/4764405/how-to-use-relative-paths-without-including-the-context-root-name
- JdbcUserRepositoryImpl.update - роли также должны обновлялться
- JdbcUserRepositoryImpl.getAll - постараться реализовать так, чтобы для 1000 пользователей был меньше, чем 1001 запрос (1 или 2).
- Для контроллера action уже не нужен - запросы нужно подкорректировать
