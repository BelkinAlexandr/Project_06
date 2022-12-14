# Проект №6 — API Testing

API  слой приложения — один из важнейших программных компонентов системы.
Он соединяет клиента с сервером (или один микросервис с другим), управляет бизнес-процессами и представляет сервисы.
API сам по себе является продуктом/сервисом.
Если он сломается, это подвергнет риску не только одно приложение, но и целую цепочку бизнес-процессов, построенных вокруг него.
Поскольку API не имеют графического интерфейса, тестирование API выполняется на уровне сообщений.
Тестирование API относится к интеграционному тестированию, а значит в ходе него можно отловить ошибки взаимодействия между модулями системы или между системами.


## Contents

1. [Chapter I](#chapter-i) \
    1.1. [API](#api)
    1.2. [Task 1](#task-api)
2. [Chapter II](#chapter-ii) \
    2.1. [REST. URL](#rest-url)
    2.2. [Task 2](#task-rest-url)
3. [Chapter III](#chapter-iii) \
    3.1. [Postman](#postman)
    3.2. [Task 3](#task-postman)
4. [Chapter IV](#chapter-iv) \
    4.1. [API Testing](#api-testing)
    4.2. [Task 4](#task-api-testing)


# Instructions

Каждую задачу данного проекта можно разделить между участниками.
Если вы еще не сделали этого в предыдущих проектах, то попробуйте такой подход к созданию документации о каком-либо изучаемом сервисе: все участники команды ищут информацию, изучают, готовят описание в установленном командой формате.
Через определенное время проводится встреча, где все участники делятся материалами и формируют одну финальную версию документа. 

Если после выполнения последнего задания в проекте вы посчитаете нужным внести корректировки в созданную документацию по предыдущим заданиям, то можете смело это делать, пока проект не завершился.

*Для выполнения тестирования вам пригодится документ HTTP из Проекта №3.*

*Все созданные документы и скрины загружайте в src ветка develop.*

*Нумерация всех скриншотов начинается с 01. В случае, если содержимое занимает больше одной страницы и требуется сделать несколько скриншотов, добавляйте дополнительную нумерацию в конец названия файла: «…_01», «…_02» и так далее.*

<h2 id="chapter-i" >Chapter I</h2>
<h2 id="api" >API</h2>

API — это акроним словосочетания Application Programming Interface (программный интерфейс приложения).

Такие интерфейсы дают возможность разным приложениям взаимодействовать между собой и обмениваться информацией.
А если совсем просто, то API предоставляет доступ к функционалу другой программы.
Например:  для интеграции с YouTube разработчику вашей компании не нужно будет создавать сложную программу.
Вместо этого можно использовать API YouTube — готовые части существующих ресурсов, у которых есть доступ к нужной вам информации и данным.
Разработчик должен настроить работу с конкретным API, для этого есть документации, в которых описываются классы, методы, переменные, константы, и приводятся функциональные примеры.

Каждый раз, когда вы делаете что-то на сайте через интернет, то вы задействуете API сервисов, которые обрабатывают ваши запросы и формируют вам ответы.



<h3 id="task-api" >Task 1</h3>

- Создайте документ «API» и заполните его информацией об API: что это такое, для чего существует, как используется и кем.  

- В документе «API» сделайте блок про тестирование API: какие существуют подходы (что такое контрактное тестирование), инструменты, какой функционал можно покрыть тестированием API.


<h2 id="chapter-ii" >Chapter II</h2>
<h2 id="rest-url" >REST. URL</h2>


REST (REpresentational State Transfer) — архитектурный стиль взаимодействия, 
который определяет, как компоненты распределенной системы должны взаимодействовать друг с другом.

В общем случае взаимодействие происходит посредством запросов-ответов.

Компоненту, которая отправляет запрос, называют клиентом; компоненту, которая обрабатывает запрос и отправляет клиенту ответ, называют сервером.
Запросы и ответы, чаще всего, отправляются по протоколу HTTP.
Сервер получает информацию о результате своего запроса с помощью кодов состояния HTTP.
Как правило, сервер — это некое веб-приложение.
Клиентом может быть, например, мобильное приложение, которое запрашивает у сервера данные, либо браузер, который отправляет запросы с веб-страницы на сервер для загрузки данных. 



<h3 id="task-rest-url" >Task 2</h3>

- Создайте файл «REST-URL». Заполните данными о URL: что такое, какова структура, в чем отличия URL и URI.

- В файл «REST-URL» добавьте данные о том, что такое REST.

- В файле «REST-URL» перечислите 6 шт. требований к архитектуре REST.

- В файле «REST-URL» опишите, что является идентификатором в REST.

- В файле «REST-UR»L добавьте блок HTTP Request-Response Structure, в котором опишите структуру HTTP запроса и ответа (это задание вам будет проще выполнить после работы в Postman в Task 4).


<h2 id="chapter-iii" >Chapter III</h2>
<h2 id="postman" >Postman</h2>

Postman — это приложение, способное выполнять запросы API к любому API HTTP. 
Postman позволяет создавать коллекции с запросами, проектировать дизайн API и создавать на его основе Mock-сервер.

<h3 id="task-postman" >Task 3</h3>

- Создайте документ «Postman». Внесите в него информацию: что такое endpoint, pre-request script, body, test.

- Скачайте и установите «Postman». Создайте личный кабинет и Workspace School21_логин-тимлида-на-платформе. Сделайте скрин, на котором видно workspace. Назовите скрин «01.postman_workspace»

<h2 id="chapter-iv" >Chapter IV</h2>
<h2 id="api-testing" >API Testing</h2>

Для проведения API тестирования в Postman используйте API и документацию https://reqres.in/

Представим такой сценарий :

- Пользователь регистрируется на сайте,
- Его данные сохраняются в бэк-енд,
- Затем данные передаются в систему, чтобы пользователь мог сделать log in без повторной регистрации.



<h3 id="task-api-testing" >Task 4</h3>

- Создайте коллекцию User_registration в Postman. Она пока пустая. 

- В созданную коллекцию добавьте POST запрос Register User. Это наш запрос №1.

- В запросе Register User заполните Url и Body. Информацию для URL запроса и его Body берем в https://reqres.in/ блок POST Register-Successful (см скрин).

![WEB](misc/images/POST_register.png)

- Запустите запрос Register User и получите токен и id пользователя. Сделайте скрин, чтобы было видно вкладку Body, статус, и в ответе — токен. Назовите скрин «02.register_user_body».

- Добавьте сохранение пользователя. Для этого в блок Tests добавьте существующий сниппет JSON value check. Откорректируйте скрипт теста чтобы получилось следующее:
`var jsonData = pm.response.json();
pm.environment.set('userId', jsonData.id);`

- Добавьте в блок Tests проверку статуса кода . Для этого в Tests добавьте существующий сниппет Code is 200.

- Запустите запрос Register User.

- Создайте GET запрос Get User с переменной userId: https://reqres.in/api/users/{{userId}}. Добавьте в Tests сниппет Code is 200. Это наш запрос №2. Запустите его.

- Добавьте Environment: userId. Зайдите в Get запрос, наведите курсором на переменную {{userId}} в запросе и сделайте скрин. Назовите скрин «03.environment». Должно быть видно, что значение userId перенесено из Environment и его значение=4 (см. скрин).

![WEB](misc/images/GET_userId.png)

- Создайте POST запрос Login User. В Body cкопируйте данные из запроса №1. Это наш запрос №3. Добавьте в Tests сниппет Code is 200.

- Реализуйте последовательность запуска коллекции. Для этого в POST запрос Login User добавьте `postman.setNextRequest('Get User');` и в POST запрос Register User добавьте `postman.setNextRequest('Login User')`.

- Сделайте запуск запроса Register User и скрин результата запуска, чтобы было видно вкладку Tests. Назовите скрин «04.register_user_test».

- Сделайте запуск запроса Login User и скрин результата запуска, чтобы было видно вкладку Tests и Body ответа. Назовите скрин «05.login_user_test».

- В GET запросе Get User укажите, что он последний (чтобы не произошел бесконечный запуск). Код для реализации этого функционала найдите самостоятельно. Сделайте запуск запроса и скрин результата запуска, чтобы было видно вкладку Tests и Body ответа. Назовите скрин «06.get_user_test».

- Запустите весь набор тестов и сделайте скрин результата запуска. Назовите скрин «07.all_tests».

<h3>Double-check</h3>
Перед загрузкой выполненного проекта в репозиторий перепроверьте наличие всех необходимых файлов, которые требовалось создать во время выполнения проекта:

- файлы:
    - «API»;
    - «REST-URL»;
    - «Postman».
- скриншоты:
    - «01.postman_workspace»;
    - «02.register_user_body»;
    - «03.environment»;
    - «04.register_user_test»;
    - «05.login_user_test»;
    - «06.get_user_test»;
    - «07.all_tests».

>Пожалуйста, оставьте обратную связь по проекту в [форме обратной связи.](https://forms.gle/C3LQFPLuLkaWPpzJA)
