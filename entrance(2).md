Java Enterprise Online Project 
===============================
Наиболее востребованные технологии /инструменты / фреймворки Java Enterprise:
Maven/ Spring/ Security/ JPA(Hibernate)/ REST(Jackson)/ Bootstrap(CSS)/ jQuery + plugins.

Вводное занятие
===============
## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) <a href="https://drive.google.com/file/d/0B9Ye2auQ_NsFSUNrdVc0bDZuX2s">Системы управления версиями. Git.

-  <a href="http://ru.wikipedia.org/wiki/Система_управления_версиями">Система управления версиями</a>. <a href="http://ru.wikipedia.org/wiki/%D0%A1%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0_%D1%83%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D1%8F_%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F%D0%BC%D0%B8#.D0.A0.D0.B0.D1.81.D0.BF.D1.80.D0.B5.D0.B4.D0.B5.D0.BB.D1.91.D0.BD.D0.BD.D1.8B.D0.B5_.D1.81.D0.B8.D1.81.D1.82.D0.B5.D0.BC.D1.8B_.D1.83.D0.BF.D1.80.D0.B0.D0.B2.D0.BB.D0.B5.D0.BD.D0.B8.D1.8F_.D0.B2.D0.B5.D1.80.D1.81.D0.B8.D1.8F.D0.BC.D0.B8">VCS/DVSC</a>.
-  Ресурсы:            
    -  <a href="https://try.github.io/levels/1/challenges/1">Интерактивная Git обучалка</a>
    -  <a href="http://githowto.com/ru">Основы Git</a>
    -  <a href="https://illustrated-git.readthedocs.org/en/latest/#working-with-remote-repositories">Working with remote repositories</a>
    -  <a href="https://www.youtube.com/playlist?list=PLIU76b8Cjem5B3sufBJ_KFTpKkMEvaTQR">Видео по обучению Git</a>
    -  <a href="http://habrahabr.ru/post/125799/">Как начать работать с GitHub: быстрый старт</a>
    -  <a href="http://ndpsoftware.com/git-cheatsheet.html">Справочник в графическом виде</a>
    -  <a href="https://blog.interlinked.org/tutorials/git.html">Git Overview</a>
    -  <a href="http://geekbrains.ru/gitstart">Видеокурс по Git</a>

##  ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZDdaaU5fZEo4X3c">Работа с проектом (выполнять инструкции)</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNHk5dVJ4N0xJTWc">prepare-to-HW0.patch (скачать и положить в каталог вашего проекта)</a>**
-  <a href="http://www.youtube.com/watch?v=_PDIVhEs6TM">Доступно о Java 8 Lambda</a>

##  Инструкция по шагам (из видео):</h3>
-  <a href="http://javawebinar.ru/#/soft">Установить ПО (git, JDK8, IntelliJ IDEA, Maven)</a>
-  Создать аккаунт на <a href="https://github.com">GitHub</a>
-  Сделать Fork ЭТОГО проекта (https://github.com/JavaOPs/topjava) </a>
-  Сделать локальный репозиторий проекта:
            <pre>git clone https://github.com/[Ваш аккаунт]/topjava.git</pre>
-  Открыть и настроить проект в IDEA
-  По ходу видео сделать Apply Patch... скаченного патча Prepare_ to_ HW0.patch
-  Закоммитить и запушить изменения (commit + push)
-  Сделать ветку домашнего задания
-  Выполнить задание и залить на GitHub (commit + push)
-  Переключиться в основную ветку проекта master.

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Домашнее задание HW0

-  <a href="http://www.mscharhag.com/2014/02/java-8-datetime-api.html">Java 8 Date and Time API</a>
-  <a href="https://drive.google.com/file/d/0B9Ye2auQ_NsFNEJWRFJkVDA3TkU/view">Time complexity</a>
-  <a href="https://ru.wikipedia.org/wiki/Временная_сложность_алгоритма">Временная сложность алгоритма</a>
-  <a href="https://ru.wikipedia.org/wiki/Вычислительная_сложность">Вычислительная сложность</a>
```
Реализовать UserMealsUtil.getFilteredMealsWithExceeded:
-  должны возвращаться только записи между startTime и endTime 
-  поле UserMealWithExceed.exceed должно показывать, 
                                     превышает ли сумма калорий за весь день параметра метода caloriesPerDay  
        
Т.е UserMealWithExceed - это запись одной еды, но поле exceeded будет одинаково для всех записей за этот день.
    
- Проверте результат выполнения ДЗ (можно проверить логику в http://topjava.herokuapp.com , список еды)
- Оцените Time complexity вашего алгоритма (если он O(N*N)- попробуйте сделать O(N).
```
Optional

-  <a href="http://devcolibri.com/4137#t2">Java 8: Lambda выражения</a>
-  <a href="http://devcolibri.com/4274#t7">Java 8: Потоки</a>
-  <a href="http://prologistic.com.ua/polnoe-rukovodstvo-po-java-8-stream.html">Pуководство по Java 8 Stream</a>
-  <a href="http://habrahabr.ru/post/224593/">Лямбда-выражения в Java 8</a>
-  <a href="http://habrahabr.ru/company/luxoft/blog/270383/">Шпаргалка Java Stream API</a>
-  <a href="http://stackoverflow.com/questions/28319064/java-8-best-way-to-transform-a-list-map-or-foreach">stream.map vs forEach</a>

```
Сделать реализация через Java 8 Stream API. Заменяйте forEach оператором stream.map(..)
```

### ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) Ваши вопросы
> Как брать диапазон дат? Какие брать дефолтные значения для null?

Для диапазона нужно использовать уже готовый `TimeUtil.isBetween`. Как приложение должно себя вести можно проверить <a href="http://topjava.herokuapp.com/">на demo</a>.

> Почему мы сначала  суммируем  калории, а потом фильтруем? Если записи за несколько лет то это лишняя работа. Не будет правильнее сначала фильтр, а потом все остальное?

На вход в getFilteredWithExceeded подается список, уже отфильтрованный по датам. Будем делать это условием в SQL.

> Лямбда выражения заменяют анонимные классы?

Синтаксически лямбду можно преобразовать в анонимный класс (в IDEA Alt+Enter на лямбде и Replace lambda with anonymous class).
Наоборот- только SAM (Single Abstract Method) интерфейс можно преобразовать в lambda. В JVM вызов происходит <a href="http://www.infoq.com/articles/Java-8-Lambdas-A-Peek-Under-the-Hood">через invokedynamic</a>.

> Как оценить временную сложность? Как определить: O(N), O(N*N) и O(N+N) ?

Из wiki это зависимость объёма работы, которая выполняется некоторым алгоритмом, от размера входных данных.
O- это коэффициент. поэтому нет O(N+N), есть O(N).
Для нашего случая все просто- если вложенный цикл или стрим, то O(N*N), иначе O(N).

> Какая сложность у map.containsKey(key)? не добрался до исходников.

Вообще исходники есть: `java.util.HashMap.containsKey`. Устройство Map (и вообще коллекции)- одни из самых частых вопросов на собеседовании.
Читаем <a href="https://habrahabr.ru/users/tarzan82/topics/">Структуры данных в картинках</a> и <a href="https://habrahabr.ru/post/162017/">Java собеседование. Коллекции</a>.
При хорошем распределении ключей сложность `HashMap.containsKey - O(1), TreeMap.containsKey - O(log2 N), а LinkedList.contains- O(N)`.

### ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Типичные ошибки в домашнем задании:
- Объявление переменных
  - <a href="https://google.github.io/styleguide/javaguide.html#s4.8.2.2-variables-limited-scope">объявляйте переменные непосредственно перед их использованием (не все вверху)</a>
  - если возможно, инициализируйте их сразу при объявлении. Если она неизменяемая, будет красиво сделать ее final.
  - рассмотрите возможность сделать ее inline (вообще без переменной). Если логика несложная, становится лаконичнее.
  - тип переменных-коллекций нужно объявлять интерфейсом: не HashMap, а Map
  - имена переменных должны быть информативные и служить заменой комментариям 

- Оформление
  - представьте, что это ваше тестовое задание на работу. Не должно быть лишних комментариев, TODO, ..
  - комментариев должен быть минимум (самодокументируемый код). Если таки нужно - лучше на english.
  - почаще пользуйтесь Ctrl+Alt+L - Reformat Code
  - в `main()` можно выводить на `System.out`. Для этого подходит перопределение `toString` объектов вывода.
