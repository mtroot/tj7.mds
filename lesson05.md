## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfmctT3oyNW1qaVhDb2p0bGpyTFVlaUJ2VVpOdVgtWF9KTUFBMWFaR2xVYVE">Материалы 5-го урока</a>

### ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Правки в проекте
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUVoyV28ybXF0ZTQ">0-fix.patch</a>**

> <a href="https://jdbc.postgresql.org/documentation/head/8-date-time.html">Новый драйвер Postgres работает с Java 8 Time API</a>, но не понимает год 0.

> Поправили в создании meals поля NOT NULL

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Разбор домашнего задания HW4

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVFVVUGctMUxxSkE">Разбор вопросов</a>
- <a href="http://stackoverflow.com/questions/8994864/how-would-i-specify-a-hibernate-pattern-annotation-using-a-regular-expression">Validate by RegExp</a>
- <a href="http://www.objectdb.com/java/jpa/persistence/managed#Entity_Object_Life_Cycle">Working with JPA Entity Objects</a>
- <a href="https://en.wikibooks.org/wiki/Java_Persistence/Relationships">Java Persistence/Relationships</a>
- <a href="http://articles.javatalks.ru/articles/17">Использование ThreadLocal переменных</a>
- <a href="http://stackoverflow.com/questions/1069992/jpa-entitymanager-why-use-persist-over-merge">Merge vs Persist</a>
- <a href="http://www.youtube.com/watch?v=1KphwODu1gg">Видео: работа в ZK с OpenJPA (в чем Hibernate хуже)</a>
- <a href="https://developer.jboss.org/wiki/OpenSessionInView">Паттерн- открытие транзакции в фильтре</a> и <a href="http://stackoverflow.com/questions/1103363/why-is-hibernate-open-session-in-view-considered-a-bad-practice">почему это bad-practice</a>
- <a href="https://en.wikibooks.org/wiki/Java_Persistence/Identity_and_Sequencing#Sequence_Strategies">Sequence Strategies</a>
- <a href="http://stackoverflow.com/questions/9470442/why-is-the-hibernate-default-generator-for-postgresql-sequencegenerator-not?lq=1">SequenceGenerator/IdentityGenerator in PostgreSql</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNFMyMGJCZWE4elk">HW4: JPA. @Rule</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFdlZoaDVlZURnTjQ">1-HW4.patch</a>**
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVDNQSmFRYUJpTDA">2-HW4-optional.patch</a>**

Изменения в проекте:

-  <a href="https://hibernate.atlassian.net/browse/HHH-8844">Add support for Java 8 date and time types (JSR-310)</a>
-  <a href="http://stackoverflow.com/questions/14892125/what-is-the-best-practice-to-determine-the-execution-time-of-the-bussiness-relev#27868954">Stopwatch</a>

## Занятие 5:
### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZENCVEhDMkZiV00">Транзакции</a>
-  <a href="https://ru.wikipedia.org/wiki/Транзакция_(информатика)">wiki Транзакция</a>
-  <a href="https://jira.spring.io/browse/DATAJPA-601">readOnly и Propagation.SUPPORTS</a>
- Ресурсы:
  - <a href="http://blog.jhades.org/how-does-spring-transactional-really-work/">How does Spring @Transactional Really Work</a>
  - <a href="https://www.ibm.com/developerworks/ru/library/j-ts1/">Стратегии работы с транзакциями: Распространенные ошибки</a>
  - <a href="http://stackoverflow.com/questions/8490852/spring-transactional-isolation-propagation">Spring @Transactional - isolation, propagation</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNW0yVWhXcGNPU2M">Профили Maven и Spring</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVTFyR0c0S1hlVjA">3-profiles-connection-pool.patch</a>**
 > Для переключения на HSQLDB необходимо:
 >  - поменять в окне Maven Projects профиль (Profiles) на `hsqldb` и сделать `Reimport All Maven Projects` (1я кнопка)
 >  - поменять в UserServiceTest/UserMealServiceTest `@ActiveProfiles(Profiles.HSQLDB)`

- <a href="https://dzone.com/articles/using-spring-profiles-xml">Using Spring Profiles in XML Config</a>
> Галочка в XML профиле влияет только на отображение в Spring и никак на выполнение кода.

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 3. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTWJOdHduOWtNcTA">Пул коннектов</a>

-  Выбор реализации пула коннектов: <a href="http://jolbox.com/">BoneCP</a>, <a href="http://commons-dbcp.apache.org">Commons Database Connection Pooling</a>, <a href="https://github.com/brettwooldridge/HikariCP">HikariCP</a>
-  <a href="http://blog.ippon.fr/2013/03/13/improving-the-performance-of-the-spring-petclinic-sample-application-part-3-of-5">Tomcat pool</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 4. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFYVdyMFYxRUR6bWM">Spring Data JPA</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFWU9mN19uemZBUFU">4-spring-data-jpa.patch</a>**

-  <a class="anchor" id="datajpa"></a><a href="http://projects.spring.io/spring-data-jpa/">Spring Data JPA</a>
-  Замена AbstractDAO: <a href="http://docs.spring.io/spring-data/jpa/docs/current/reference/html/#jpa.repositories">JPA Repositories</a>
-  Разрешение зависимостей: <a href="http://howtodoinjava.com/2014/02/18/maven-bom-bill-of-materials-dependency/">Maven BOM [Bill Of Materials] Dependency</a>
-  <a href="http://habrahabr.ru/post/232381/">Делегирование. (Spring Data JPA)</a>
-  <a href="http://docs.spring.io/spring-data/jpa/docs/current/reference/html/#jpa.query-methods.query-creation">Query methods</a>
-  <a href="http://jeeconf.com/archive/jeeconf-2013/materials/spring-data/">Spring Data – новый взгляд на persistence (JeeConf)</a>

-  Ресурсы:
   -  <a href="https://github.com/spring-projects?query=spring-data">Github repositories</a></li>
   -  <a href="http://www.petrikainulainen.net/spring-data-jpa-tutorial">Spring Data JPA Tutorial</a></li>
   -  <a href="https://blog.42.nl/articles/spring-data-jpa-with-querydsl-repositories-made-easy/">Spring Data JPA with QueryDSL</a></li>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 5. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFajd2Y2RLQVVJWUU">Spring кэш</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFRXpnNjhVdkJDc2M">5-spring-cache</a>**

-  <a href="http://habrahabr.ru/post/113945/">Кеширование в Spring Framework</a>
-  <a href="http://www.ehcache.org/">EHCACHE</a>
-  В случае проблем с резмещением кэш в `java.io.tmpdir`: http://stackoverflow.com/questions/1924136/environment-variable-to-control-java-io-tmpdir

-  Ресурсы:
   -  <a href="http://docs.spring.io/spring-framework/docs/current/spring-framework-reference/html/cache.html">Spring cache Abstraction</a>
   -  <a href="http://habrahabr.ru/post/25140/">Распределённая система кеша ehcache</a>
   -  Починка JUnit: <a href="http://stackoverflow.com/questions/10013288/another-unnamed-cachemanager-already-exists-in-the-same-vm-ehcache-2-5">один кэш на JVM</a>

--------------------

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZFdWWFdwams0eGM">Домашнее задание HW05</a>
     Имплементировать DataJpaUserMealRepositoryImpl
     Разделить реализации Repository по профилям Spring: jdbc, jpa, datajpa
            (общее в профилях можно объединять, например <beans profile="datajpa,jpa">)
     Сделать тесты всех реализаций (jdbc, jpa, datajpa) через наследование (без дублирования),
             общее из UserMealServiceTest и UserServiceTest вынеси в базовый класс.
     Запустить все тесты: mvn test
                          или в IDEA Maven Lifecycle- test (кнопку skipTest отжать)

Optional

     Починить MealServlet / SpringMain (добавить профили. 
                      Попробуйте поднять Spring контекст без использования `spring.profiles.activ`).

     Сделать и протестировать в сервисах методы (можно сделать разные варианты, реализация только в DataJpa):
     -  достать по id пользователя вместе с его едой
     -  достать по id еду вместе с пользователем
     Обращения к DB сделать в одной транзакции
     
     Почините JDBC реализацию для HSQLDB, можно также разнести ее по профилям.

## ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) Ваши вопросы
> В <a href="https://github.com/spring-projects/spring-petclinic/tree/master/src/main/java/org/springframework/samples/petclinic/repository/springdatajpa">spring-petclinic</a> DataJpa реализована без проксирования и без доп. классов. В таком виде как у них, spring data смотрится, конечно, намного лаконичней других реализаций, но у нас получилось  вдвое больше кода, чем с тем же jpa или jdbc. Плюс только пожалуй в том, что query находятся прямо в репозитории, а  не где-то там в другом пакете. Так что получается, spring data лучше подходит для простейших crud без всяких "фишек"? или в чем его достоинство для больших и сложных проектов?

Достоинство DATA-JPA по сравнению например с JPA: есть типизация, готовые реализации типовых методов CRUD а также paging, data-common. Мы можем переключить реализацию JPA, например, на mongoDb (PagingAndSortingRepository, от которого наследуется JpaRepository находится в `spring-data-common`).
Соответственно его методы будет поддерживаться всеми реализациями spring-data-common, JPA одна из них и пр. Подробнее о них есть в видео <a href="http://jeeconf.com/archive/jeeconf-2013/materials/spring-data/">Spring Data – новый взгляд на persistence</a>.
Я сам ввел дополнительное проксирование для устранения минусов подхода DATA-JPA: невозможность дебага и привязка к интерфейсу JpaRepository.
Приложение становится больше, но выигрыш этого стоит. Можно не делать дополнительный класс и перенести его логику в слой сервиса.

> Почему мы для InMemory не сдалели отдельного профиля? Почему их не удалить вообще?

Реализация InMemory является примером как в test делать моки с подменой контекста. Для них сделали отдельный `mock.xml` и запускаемый проект ничего не должен о них знать. У нас учебный проект, в котором 4 реализации репозиториев, в реальном такого не будет.

---------------------
### ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Подсказки по HW05
- Для того, чтобы не запускались родительские классы тестов нужно сделать их `abstract`
- Для IDEA не забудте выставить в `spring-db.xml` справа вверху в Change Profiles... профили, например `datajpa, postgres`
- Общие части для всех в `spring-db.xml` можно оставить как есть без профилей, но до первого `<beans profile=` (вверху файла).
- В MealServlet/SpringMain в момент `setActiveProfiles` контекст спринга еще не должен быть инициализирован, иначе выставление профиля уже ничего не будет делать.
- Если у метода нет реализации, то стандартно бросается `OperationNotSupportedException`.
- Для уменьшения количества кода при реализации Optional попробуйте сделать default метод в интерфейсе
