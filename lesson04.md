## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfkxqbVpwZUd5anQ2TXE4bm5HbXhtVmkxMUxFSjhNQ1hXYVVTTTZEMzkzN2s">Материалы 4-го урока</a>

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Разбор домашнего задания HW3
> SpringMain/ InMemory*Test починим в видео 3, `5-create-mock-test-ctx.patch`

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFdVhaMklZQVNkUGc">JdbcUserMealRepositoryImpl + UserMealServiceTest</a>
- <a href="http://www.techonthenet.com/postgresql/between.php">POSTGRESQL: BETWEEN CONDITION</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFeW1lR0JwY2ZpWHc">1-HW3.patch</a>**

> Новый Postgres драйвер <a href="https://jdbc.postgresql.org/documentation/head/8-date-time.html">поддерживает Java 8 Date and Time</a>. Преобразования c Timestamp оказались уже не нужны. Мне кажется хороший пример того, что все надо проверять самим, а не верить на слово:)

- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSlJUM1hTM0lwMWc">2-HW3-optional.patch</a>**

> В JUnit тестах используется кодировка по умолчанию и тесты, если их запускать через maven, не проходят. Решается кастомизацией плагина <a href="https://maven.apache.org/surefire/maven-surefire-plugin/">maven-surefire-plugin</a>

> В meals добавил составной индекс `INDEX meals_unique_user_datetime_idx ON meals(user_id, date_time)`:
 - все запросы в таблицу meals у нас идут с `user_id`
 - по полю `date_time` также есть запросы + мы по нему сортируем список результатов
 те они- хорошие кандидаты для индексирования. <a href="http://stackoverflow.com/questions/970562/postgres-and-indexes-on-foreign-keys-and-primary-keys">На id как на primary key индекс создается автоматически</a>.

## ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) Вопросы по HW3

> Почему в meals дата и каллории у нас не NOT NULL? Это ведь обязательные для заполнения поля.

Спасибо, недосмотр. Сделаем NOT NULL в HW04.


## Занятие 4:
### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFU005ZzBNZmZnTVU">Методы улучшения качества кода</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQVFxSUdpLUd1WE0">3-improve-code.patch</a>**
- <a href="https://ru.wikipedia.org/wiki/Контрактное_программирование">Контрактное программирование</a>, <a href="http://neerc.ifmo.ru/wiki/index.php?title=Программирование_по_контракту">Программирование по контракту</a>
- <a href="http://www.sw-engineering-candies.com/blog-1/comparison-of-ways-to-check-preconditions-in-java">Comparison Preconditions in Java</a>
- <a href="https://code.google.com/archive/p/findbugs/wikis/IntellijFindBugsPlugins.wiki">QAPlug vs FindBugs</a>
- <a href="http://qaplug.com/about/tutorials/">QAPlug tutorials</a>
- <a href="https://www.codacy.com">Codacy Home</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFU0Z2R190eDllYmM">Spring: инициализация и популирование DB</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQVNzRl9oS2I5VTA">4-init-and-populate-db.patch</a>**
> - `@Sql` в тестах заменяет `@Before public void setUp()`, те выполняется перед каждым тестом

-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/jdbc.html#jdbc-initializing-datasource-xml">Инициализация базы при старте приложения</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/htmlsingle/#integration-testing-annotations-spring">Spring Testing Annotations</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/htmlsingle/#resources">Абстракция Resource</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 3. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNTNWV04weDBGSmc">Починка SpringMain/ InMemory*Test: подмена контекста при тестировании</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUVhpUTBMQ0dsNnM">5-create-mock-test-ctx.patch</a>**

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 4. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVWZYcHoyUF9qX2M">ORM. Hibernate. JPA.</a>
> ВНИМАНИЕ: патч меняет postgres.properties, в котором у вас свои креденшелы к базе.

> Тесты и приложение ломаются. `UserMealServiceTest` починится после выполнения HW04 (`JpaUserMealRepositoryImpl`)

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFT0JoR0I1UGxycnc">6-add-jpa.patch</a>**
>  Upgrade Hibernate to 5.0.4 needed to add `javax.transaction.jta`, see <a href="https://hibernate.atlassian.net/browse/HHH-10307">5.0.4 requires javax.transaction.SystemException</a>
>  Upgrade Hibernate Validator needed to add `javax.el-api`, see <a href="http://stackoverflow.com/questions/24386771/javax-validation-validationexception-hv000183-unable-to-load-javax-el-express">javax.validation.ValidationException</a>

-  <a href="http://ru.wikipedia.org/wiki/ORM">ORM</a>.
-  <a href="http://habrahabr.ru/post/265061/">JPA и Hibernate в вопросах и ответах</a>
-  <a href="http://www.quizful.net/post/Hibernate-3-introduction-and-writing-hello-world-application">Hibernate: введение и написания Hello world приложения</a>
-  <a href="http://en.wikibooks.org/wiki/Java_Persistence/Mapping">Mapping</a>. Описания модели Hibernate (hbm.xml/annotation)
-  <a href="https://ru.wikipedia.org/wiki/Hibernate_(библиотека)">Hibernate</a>. Другие ORM: <a href="http://en.wikipedia.org/wiki/TopLink">TopLink</a>, <a href="http://en.wikipedia.org/wiki/EclipseLink">ElipseLink</a>, <a href="http://en.wikipedia.org/wiki/Ebean">EBean</a> (<a href="http://www.playframework.com/documentation/2.2.x/JavaEbean">used in Playframework</a>).
-  <a href="http://ru.wikipedia.org/wiki/Java_Persistence_API">JPA (wiki)</a>. <a href="https://en.wikipedia.org/wiki/Java_Persistence_API">JPA (english wiki)</a>. <a href="http://www.jpab.org/All/All/All.html">JPA Performance Benchmark</a>
-  Подключение к проекту Spring ORM и Hibernate
-  <a href="http://en.wikibooks.org/wiki/Java_Persistence/Inheritance">Отображения наследования объектов на таблицы</a>
-  <a href="http://en.wikibooks.org/wiki/Java_Persistence/Identity_and_Sequencing">Стратегии генерации PK</a>
-  Добавление <a href="http://validator.hibernate.org">hibernate-validator</a>. <a href="http://stackoverflow.com/questions/14730329/jpa-2-0-exception-to-use-javax-validation-package-in-jpa-2-0">JSR-303 -> JSR-349</a>
-  <a href="http://devcolibri.com/2046">Описание связей в модели. Ленивая загрузка объекта.</a>
-  Конфигурирование JPA. Сканировние Entities. <a href="http://docs.jboss.org/hibernate/entitymanager/3.6/reference/en/html/architecture.html#d0e61">JPA definitions</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/expressions.html">Spring expressions: выражения в конфигурации</a>
-  Создание JPA Facet. Назначение DataSource.
-  Имплементация JpaUserRepository через EntityManagerFactory/ SessionFactory
-  Использование TypedQuery и @NamedQuery. Назначение параметров по индексу и имени.
-  <a href="http://docs.jboss.org/hibernate/orm/4.2/devguide/en-US/html/ch11.html">HQL</a>/ <a href="http://ru.wikipedia.org/wiki/Java_Persistence_Query_Language">JPQL</a>.
-  <a href="http://www.objectdb.com/java/jpa/query/criteria">JPA Criteria API</a>. <a href="http://www.querydsl.com/">Unified Queries for Java</a>
-  <a href="https://weblogs.java.net/blog/montanajava/archive/2014/06/17/using-java-8-datetime-classes-jpa">Java 8 Time API Converter</a>

- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFdFl0MXFvZ1NaWFE">7-add-named-query-and-transaction.patch</a>**
-  <a href="http://ru.wikipedia.org/wiki/Транзакция_(информатика)">Транзакция. ACID. Уровни изоляции транзакций.</a>
-  Подключаем транзакции. <a href="http://www.tutorialspoint.com/spring/spring_transaction_management.htm">Spring Transaction Management</a>
-  <a href="https://jira.spring.io/browse/DATAJPA-601">readOnly и Propagation.SUPPORTS</a>
-  <a href="http://habrahabr.ru/post/232381/">@Transactional в тестах. Настройка EntityManagerFactory</a>

-  Справочник:
   - <a href="http://www.youtube.com/watch?v=YzOTZTt-PR0">Николай Алименков — Босиком по граблям Hibernate</a>
   - <a href="http://www.byteslounge.com/tutorials/spring-transaction-propagation-tutorial">Spring transaction propagation tutorial</a>
   - <a href="https://dzone.com/refcardz/getting-started-with-jpa">Getting Started with JPA</a>
   - <a href="http://stackoverflow.com/questions/8994864/how-would-i-specify-a-hibernate-pattern-annotation-using-a-regular-expression">Validate by RegExp</a>
   - <a href="http://en.wikibooks.org/wiki/Java_Persistence">Java Persistence</a>
   - <a href="http://hibernate.org/">Hibernate</a>
   - <a href="http://docs.spring.io/spring-framework/docs/4.0.x/spring-framework-reference/html/transaction.html">Spring Framework transaction management</a>
   - <a href="http://www.objectdb.com/java/jpa/persistence/managed#Entity_Object_Life_Cycle">Working with JPA Entity Objects</a>
   - <a href="http://www.ibm.com/developerworks/ru/library/j-ts1/">Стратегии работы с транзакциями: Распространенные ошибки</a>
   - <a href="http://habrahabr.ru/post/208400/">Принципы работы СУБД. MVCC</a>
   - <a href="https://ru.wikipedia.org/wiki/MVCC">MVCC</a>


###  ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 5. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSTJEQ1Rvd3Jvc2c">Добавляем поддержку HSQLDB</a>

- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNE9lNlhFTEx0ZTA">8-add-hsqldb.patch</a>**

>  ВНИМАНИЕ: патч меняет postgres.properties

> IDEA может `${jdbc.initLocation}` подчеркивать красным - иногда тупит...

## ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) Ваши вопросы

>  Есть несколько аналогичных "встроенных" баз данных. H2, HSQLDB, Derby, SQLite. Почему был выбран HSQLDB?

Просто с ней приходилось работать. HSQLDB и H2 наиболее популярны, в новом курсе по spring-boot планирую использовать H2.

> Чистого JPA не существует, т.е. это всего лишь интерфейс, спецификация? Говорим JPA, подразумеваем какой-то ORM фрэймворк? А что тогда используют чистый jdbc, Spring-jdbc, MyBatis? MyBatis не реализует JPA?

JPA- это спецификация, API. Ее реализации- Hibernate, OpenJPA, EclipceLink. Spring-Jdbc, MyBatis, db-utils не реализуют JPA, это обертки к JDBC. Все ORM также реализованы поверх JDBC.

> В зависимостях maven `hibernate-entitymanager` тянет за собой `jboss-logging`. Как будет происходить логгирование?

<a href="http://stackoverflow.com/questions/11639997/how-do-you-configure-logging-in-hibernate-4-to-use-slf4j">How do you configure logging in Hibernate 4 to use SLF4J</a>: в нашем проекте автоматически подхватывается `logback-classic`.

--------------------

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Домашнее задание HW04

    Сделать UserMeal как Hibernate entity
    Добавить поддержку LocalDateTime
    Имплементировать и протестировать JpaUserMealRepositoryImpl

-  IDEA не понимает в @NamedQuery `..  m.dateTime BETWEEN ..`. На функциональность это не влияет.
-  <a href="http://stackoverflow.com/questions/23718383/jpa-support-for-java-8-new-date-and-time-api">JPA support for Java 8 new date and time API</a>
-  <a href="http://stackoverflow.com/questions/31965179/whats-new-in-hibernate-5">What's new in Hibernate 5?</a>

Optional 

    Добавить в тесты UserMealServiceTest функциональность @Rule:
     - проверку Exception
     - вывод в лог времени выполнения каждого теста

-  <a href="https://github.com/junit-team/junit/wiki/Rules">JUnit @Rules</a>

---------------------
### ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Подсказки по HW04

-  Тк. JPQL работает с объектами мы не можем использовать userId для сохранения. Можно сделать например так:

        User ref = em.getReference(User.class, userId);
        meal.setUser(ref);

   При этом от User нам нужет только id, т.е. реального запроса в базу за юзером не будет- проверьте по логам Hibernate.

- В JPQL запросах можно писать: `m.user.id=:userId`

- При реализации `JpaUserMealRepositoryImpl` предпочтительно не использовать try-catch в логике реализации. Но если очень хочется, то ловить только специфичекские эксепшены (пр. `NoResultException`), чтобы, например, при отсутствии коннекта к базе приложение отвечало адекватно.

- Мы будем смотреть генерацию db скриптов из модели, для корректоной генерации нужно в `UserMeal` добавить `uniqueConstraints`
