## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfk43cG91Yk9pM3JxUHVhNFVVdHlxSlJtZm5oY3A4YXRtNk1KWEZxRlFNeW8">Материалы 10-го урока</a>

### ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Правка кода
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFME50SGUtR053T1U">0-fix.patch</a>**
- Добавил в fail детали `jqXHR.responseJSON`
- Упростил callback для `updateTableByData`
- Поправил html и import

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Разбор домашнего задания HW9

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZnQ2dDZsT0dvYjQ">HW9</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFU1NoNEJnTFJDbjQ">1_HW9_ajax.patch</a>**

> Добавил UserMealTo (раньше был вместе с entity)

- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFd1pEUEdfd3g2Ukk">2_HW9_test.patch</a>**
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZFVpTmhuRGlmaGM">3_HW9_datetimepicker.patch</a>**

> Изменил формат ввода даты в форме без 'T'

  - <a href="http://xdsoft.net/jqplugins/datetimepicker/">DateTimePicker jQuery plugin</a>
  - <a href="https://github.com/xdan/datetimepicker/issues/216">Datetimepicker and ISO-8601</a>

## Занятие 10:

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTVZyQnBlYUtkNms">Spring Security Taglib. Method Security Expressions.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSjNkbFRicEtBWnc">04_secure_tag_annotation.patch</a>**
-  <a href="http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#declaring-the-taglib">Spring Security Taglib.</a>
-  <a href="http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#jc-method">Method Security</a> и <a href="http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#method-security-expressions">Method Security Expressions</a>. Зависимость от контекста mvc/parent.

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2.  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFc1JMTE4xVG0zN0U">Interceptors. Редактирование профиля. JSP tag files.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFd0ptVDBEcjlmS2M">05_interceptor.patch</a>**
-  Добавляем профиль. <a href="http://www.mkyong.com/spring-mvc/spring-mvc-handler-interceptors-example/">Spring interceptors</a>.
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFS3k0UXpXdlJ3bGM">06_profile_jsptag.patch</a>**

>  ProfileRestController.update(user) изменился на userTo (нельзя, например, изменять себе роли).

-  <a href="http://www.techrepublic.com/article/an-introduction-to-jsp-20s-tag-files/">Делаем jsp tag для ввода поля формы</a>.
-  <a href="http://www.codejava.net/frameworks/spring/spring-mvc-form-validation-example-with-bean-validation-api">Spring MVC Form Validation</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 3. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNWpUNktMeGJURmM">Форма регистрации.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZDgxX1dCZncyMWs">07_registration.patch</a>**

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 4. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFODlhSTZnLXZzaHc">Обработка исключений в Spring.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTGFuWVpPbFNOYnM">08_not_found_404.patch</a>**
-  <a href="http://spring.io/blog/2013/11/01/exception-handling-in-spring-mvc#using-http-status-codes">Используем HTTP status code</a>
-  <a href="http://stackoverflow.com/questions/2195639/restful-resource-not-found-404-or-204-jersey-returns-204-on-null-being-returne">RESTful resource not found</a>
-  <a href="http://stackoverflow.com/questions/9930695/rest-api-404-bad-uri-or-missing-resource">REST API 404</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFbVpHaWxBWUNjb00">9_global_exception.patch</a>**
-  <a href="http://spring.io/blog/2013/11/01/exception-handling-in-spring-mvc#global-exception-handling">Global Exception Handling</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFbzBtYnpvR2tfa2M">10_controller_based_exception.patch</a>**

>  Т.к Rest и Ajax контроллеры уже отнаследованы от абстрактных контроллеров, сделал "подмешивание" в них ExceptionInfoHandler с помощью default методов интерфейса.

-  <a href="https://ru.wikipedia.org/wiki/Примесь_(программирование)">Примесь (mixin)</a>
-  <a href="https://kerflyn.wordpress.com/2012/07/09/java-8-now-you-have-mixins/">Mixin в Java 8</a>
-  <a href="http://spring.io/blog/2013/11/01/exception-handling-in-spring-mvc#errors-and-rest">Сериализация Exception в JSON</a>
-  <a href="http://spring.io/blog/2013/11/01/exception-handling-in-spring-mvc#controller-based-exception-handling">Exception Handling на уровне контроллера</a>


### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 5. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUHNiYzNMbkF6ajQ">Encoding password</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTVRISUR6OEN3Tzg">11_password_encoding.patch</a>**
- <a href="http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#core-services-password-encoding">Password Encoding</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 6. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNDlPZGdUNThzNUU">Межсайтовая подделка запроса (CSRF).</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUTg2c1R4WTQycXc">12_csrf.patch</a>**
-  <a class="anchor" id="csrf"></a><a href="https://ru.wikipedia.org/wiki/Межсайтовая_подделка_запроса">Межсайтовая подделка запроса (CSRF)</a>
-  <a href="http://docs.spring.io/spring-security/site/docs/current/reference/html/csrf.html#csrf-using/">Using Spring Security CSRF Protection</a>
-  <a href="http://docs.spring.io/spring-security/site/docs/current/reference/html/csrf.html#csrf-include-csrf-token-ajax">Ajax and JSON Requests</a>
-  <a href="http://blog.jdriven.com/2014/10/stateless-spring-security-part-1-stateless-csrf-protection/">Stateless CSRF protection</a>
-  Ресурсы:
    -  <a href="http://habrahabr.ru/post/264641/">Spring Security 4 + CSRF</a>
    -  <a href="http://stackoverflow.com/questions/11008469/are-json-web-services-vulnerable-to-csrf-attacks">Are JSON web services vulnerable to CSRF attacks</a>
    -  <a href="https://ru.wikipedia.org/wiki/Правило_ограничения_домена">Правило ограничения домена (SOP)</a>
    -  <a href="https://ru.wikipedia.org/wiki/Cross-origin_resource_sharing">Cross-origin resource sharing (CORS)</a>

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Домашнее задание HW10
    Сделать валидацию в AdminAjaxController/UserMealAjaxController через ValidationException
    (вернуть клиенту ErrorInfo и статус HttpStatus.UNPROCESSABLE_ENTITY)

    Сделать обработку ошибки при дублирования email (User with this email already present in application) для: 
         регистрации / редактирования профиля пользователя
         добавления / редактирования пользователя в списке
    

Optional.

    Сделать в приложении выбор локали (см. http://topjava.herokuapp.com/)

    Починить UTF-8 в редактировании профиля и регистрации (в windows). Подумайте, почему они поломались.

Ресурсы:
-  <a href="http://www.mkyong.com/spring-mvc/spring-mvc-internationalization-example">Spring MVC internationalization sample</a>
-  <a href="http://www.concretepage.com/spring-4/spring-4-mvc-internationalization-i18n-and-localization-l10n-annotation-example">Spring 4 MVC Internationalization</a>

## ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) Ваши вопросы

> В чем отличие между аннотоацией `@PreAuthorize("hasRole('ROLE_ADMIN')")` и конфигурацией в jsp: `<sec:authorize access="isAuthenticated()">`, `<sec:authorize access="hasRole('ROLE_ADMIN')">` ?

Анотация `@PreAuthorize` обрабатывается Spring анологично `@Transactional`, `@Cacheable` - класс проксируется и до-после вызова метода добавляется функциональность.
В данном случае перед вызовом метода проверяются роль залогиненного юзера. JSTL тэг `authorize` выполняет проверку условия в залогиненном юзере внутри jsp.

> Какой из `SessionLocaleResolver` и `CookieLocaleResolver` а какой лучше использовать для локализации?

Я взял `CookieLocaleResolver`. Он хранит информацию в куках, которые хранятся долго у клиента на компьютере. Локаль в сессии проподает вместе с логаутом.
