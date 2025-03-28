# Сайт генерації QR кодів / QR code generation site

---

## Навігація:

- [Мета додатку / Purpose of the application](#мета-додатку--purpose-of-the-application)
- [Склад команди / Team members](#склад-команди--team-members)
- [Використані технології / Tehnologies used](#використані-технології--technologies-used)
- [Інструкції / Instructions](#інструкції--instructions)
- [Структура / Structure](#структура--structure)
- [Структура додатків / Application structure](#структура-додатку--application-structure)
- [Додатки / Applications](#додатки--applications)
- [Особливості роботи додатку / Features of the application](#особливості-роботи-додатків--features-of-the-applications)
- [Посилання / Links](#посилання--links)
- [Висновок / Conclusion](#висновок--conslusion)

---

## Мета додатку / Purpose of the application:
#### Цей проект дозволяє користувачам цього сайту створювати QR коди з можливвстю кастомизації та онлайн сховища QR кодів! / This project allows users of this site to create QR codes with the possibility of customization and online storage of QR codes!
#### А для вас, як для хосту сайту, буде можливість місячного заробітку викоритовуючи підписки для користувачів на сайті! / And for you, as the site host, there will be an opportunity to earn monthly income using subscriptions for users on the site!

---

## Склад команди / Team members:
0. [Терешонок Максим](https://github.com/TereshonokMaksim/QR-Code-Generator) - Тімлід команди / Team leader
1. [Агеєв Данило](https://github.com/Ageev-Danilo/QR-Code-Generator)
2. [Олефіренко Глеб](https://github.com/GlebOlefirenko/QR_Generator)

---

## Використані технології / Technologies used:
### Python
#### Це, мова програмування на якій працює практично все на бекенду / This is the programming language that runs almost everything on the backend.
_Нижче, будуть приведені фреймворки які були використані для створення бекенду / Below, the frameworks that were used to create the backend will be listed._
1. Django - Фреймворк, який, в нашому проекті, використовувався для роботи з цілим проектом на стороні серверу (бекенду) та для більш зручної праці з базами даних. Також, його шаблонізатор відповідає за динамічний контент веб-сторінок. / Django - A framework that, in our project, was used to work with the entire project on the server side (backend) and for more convenient work with databases. Also, its templating engine is responsible for dynamic content of web pages.
2. Pillow (PIL) - бібліотека, котра довзоляє працювати с зображеннями. За допомогою неї корегується QR код під налаштування користувача. / A library that allows you to work with images. It is used to adjust the QR code to the user's preferences.
3. qrcode - бібліотека, яке генерує QR код з тексту, який вводить користувач. / a library that generates a QR code from text entered by the user.
4. datetime - бібліотека, яке довзоляє швидко та зручно працювати з часом, необхідно для роботи з підписками. / A library that allows you to quickly and conveniently work with time is necessary for working with subscriptions.
### HTML 5
#### Мова-конструктор, на якому побудована структура всіх веб-сторінок проекту. Його робота підкріплювалася зі сторони бекенду за допомогою шаблонізатору Django. / A construction language that built the structure of all the project's web pages. Its work was supported on the backend side using the Django templating engine.
### CSS
#### Мова для надання сторінкам стилів і деякого косметичного функціоналу / A language for giving pages styles and some cosmetic functionality
### JavaScript (JS)
#### Мова для створення інтерактивності веб-сторінок, відповідає за відправку даних без оновлення сторінки (XML запити) / Language for creating interactivity on web pages, responsible for sending data without refreshing the page (XML queries)
### Бази Даних / DataBases
#### Вони використовувались для зручної зберігання великих об'ємів даних користувачів, підписок та QR кодів.
### git
#### Він використовувся для організації командної роботи учасників за допомогою гілок та відслідковування версій додатку.
### Figma
#### Вона використовувався для створення дизайну, створенню схеми бази даних та схематичному розподілу праці учасників.

---

## Інструкції / Instructions

<details>

<summary>Натисніть, щоб побачити інструкцію по запуску та обслуговуванню проекту / Click to see instructions for launching and maintaining the project</summary>

Рекомендується виконати всі інструкції, якщо ви хочете мати працюючий проект / It is recommended to follow all instructions if you want to have a working project.

---

<details>
<summary>Натисніть, щоб побачити інструкцію по запуску проекту / Click to see instructions for starting the project</summary>

### Як запустити проект ЛОКАЛЬНО / how to launch project LOCALLY

1. >Переконайтесь, що ви маєте версію Python >=3.11 з встановленим PIP (Package Installer for Python) / Make sure you have Python version >3.11 with PIP (Package Installer for Python) installed
2. >Встановіть цей проект собі на комп'ютер. Для цього, наведіться на зелену кнопку "<> Code" та натисність на найнижчу відкриту кнопку "Download ZIP" / Install this project on your computer. To do this, hover over the green "<> Code" button and click on the lowest open button "Download ZIP"
3. >Розархівуйте встановлену ZIP папку / Unzip the installed ZIP folder
4. >Відкрийте командний рядок у себе на комп'ютері та перейдіть у папку с проектом. Для цього відкрийте командний рядок у цій самий папці, або перейдіть у неї користуючись командою cd / Open a command prompt on your computer and navigate to the project folder. To do this, open a command prompt in the same folder, or navigate to it using the cd command.
5. >Коли ви перейшли у QR_Code_Generator, напишіть цю команду / When you are in QR_Code_Generator, write this command:
```bash
    pip install -f requirements.txt
    # Це встановить всі залежності у проекта (всі бібліотеки, які потрібні для нормальної роботи програми) / This will install all dependencies for the project (all libraries that are required for the program to work properly)
```
6. >Перейдіть у папку QR_Generator так, щоб вам був доступний файл manage.py (все ще за допомогою команди "cd") / Go to the QR_Generator folder so that you have access to the manage.py file (still using the "cd" command)
7. >Створіть базу даних проекту / Create a project database:
```bash
    python manage.py migrate
    # Це проведе міграції бази даних - створить всі моделі проекту та зробе його базу даних працюючою / This will perform database migrations - create all project models and make its database working
```
i. >Якщо ви маєте помилку (багато незрозумілого тексту) після використання цієї команди, використайте її ще раз, після виконання наступної команди / If you get an error (a lot of garbled text) after using this command, use it again, after running the following command:
```bash
    python manage.py makemigrations
    # Це створить міграції для бази даних. / This will create migrations for the database.
```
8. >Запустість проект / Run project:
```bash
    python manage.py runserver
    # Це запустить проект локально / This will run project locally
```
i. Якщо виникають помилки, переконайтеся, що ви не пропустили минулих пунктів / If errors occur, make sure you haven't missed any previous points.
#### Для продовження налаштування проекту, відкрийте інструкцію по обслуговуванню проекта / To continue configuring the project, open the project maintenance manual.
</details>

<details>
<summary>Натисніть, щоб побачити інструкцію по обслуговуванню проекту / Click to see the project maintenance instructions</summary>

### Інструкція по обслуговуванню сайту ЛОКАЛЬНО / Instruction how to manage site LOCALLY

1. >Переконайтеся, що ви маєте створений проект по інструкції з запуску проекту / Make sure you have a project created according to the project launch instructions
2. >Для створення першого адміністратора сторінки, переконайтеся що ви у папці с manage.py та використайте цю команду / To create the first page administrator, make sure you are in the folder with manage.py and use this command:
```bash
    python manage.py createsuperuser  
    # Після запуску цієї команди, вам будуть поставлені декілька запитань, а саме: юзер нейм, електронна пошта та пароль від вашого акаунту адмінстратора / After running this command, you will be asked several questions, namely: username, email, and password for your administrator account.
    # Важливо: Коли ви будете вводити пароль, він не буде виводитиь у консоль, тому це важливо його запам'ятати або скопіювати / Important: When you enter your password, it will not be displayed in the console, so it is important to remember or copy it.
```
3. >Запустіть проект (сервер) по пункту 8 з інструкції запуску проекту / Start the project (server) according to step 8 of the project launch instructions.
4. >Відкрийте посилання котре виведе в консоль (зазвичай це "http://127.0.0.1:8000/") / Open the link that will output to the console (usually "http://127.0.0.1:8000/")
5. >У кінець адресного рядка введіть "admin" (зазвичай вийде "http://127.0.0.1:8000/admin/") / At the end of the address bar, type "admin" (usually it will be "http://127.0.0.1:8000/admin/")
6. >Введіть ваш юзернейм та пароль у відповідні поля / Enter your username and password in the appropriate fields.
7. >Створіть першу підписку / Create your first subscription:
    1. Відкрийте Subscriptions  у відкрившомуся сторінці адміністратора / Open Subscriptions in the opened admin page
    2. Натисніть "ADD SUBSCRIPTION" / Click "ADD SUBSCRIPTION"
    3. У якості імені (Title) обов'язково введіть "Free" (тільки для першої підписки - вона необхідна для роботи всієї системи підписок) / Be sure to enter "Free" as the Title (only for the first subscription - it is necessary for the entire subscription system to work)
    4. Введіть відповідні значення у поля Description (коротко), Price, Max qrcodes / Enter the appropriate values ​​in the Description (short), Price, Max qrcodes fields
    5. Якщо ви хочете створити підписку, котра буде доступна тільки адміністраторам, ввимкніть Visible (натисніть по галочці) / If you want to create a subscription that will only be available to administrators, turn off Visible (click the check mark)
7. >Для того, щоб ваш акаунт адміністратора міг користуватися сайтом, виконайте наступну послідовність дій / To enable your administrator account to use the site, follow these steps::
    1. Відкрийте Accounts на сторінці адміністратора / Open Accounts on the admin page
    2. Натисніть "ADD ACCOUNT" / Click "ADD ACCOUNT"
    3. У якості User виберіть свій поточний акаунт / As User, select your current account
    4. У поле Verified введіть 1 / In Verified field enter 1
    5. У Subscription виберіть нещодавно створену підписку / Under Subscription, select the newly created subscription
8. >Якщо ви хочете видалити об'єкти будь якої моделі, виконайте наступну послідовність подій / If you want to delete objects from any model, follow the following sequence of events:
    1. Відкрийте модель за допомогою натискання на неї на сторінці адміністратора / Open the model by clicking on it on the admin page
    2. Виберіть об'єкти за допомогою натискання на квадратик зліва від назви об'єкта / Select objects by clicking on the box to the left of the object name.
    3. У полі вибору біля тексту Action виберіть "Delete selected {назва моделі}s" та натисність "Go" / In the selection box next to the Action text, select "Delete selected {model name}s" and click "Go"
i. Рекомендовано створювати QR коди тільки на сторінці створення QR кода, намагайтеся не користуватися сторінкою адміністрації для цього / It is recommended to create QR codes only on the QR code creation page, try not to use the administration page for this
</details>
</details>

---

## Структура / Structure

<details>
<summary>Натисніть, щоб побачити схематичну структуру проекту / Click to see the schematic structure of the project</summary>

```mermaid
%%{ init : { "theme" : "default", "flowchart" : { "curve" : "linear" } }}%%

flowchart LR

    A(QR_Generator_main) --> L(QR_Generator)
    A(QR_Generator_main) --> K(home_app)
    A(QR_Generator_main) --> J(qrcode_app)
    A(QR_Generator_main) --> I(user_app)
    A(QR_Generator_main) --> H(contacts_app)
    A(QR_Generator_main) --> G(media)
    A(QR_Generator_main) --> F(templates)
    A(QR_Generator_main) --> E(Static Base)
    A(QR_Generator_main) --> D([db.sqlite3])
    A(QR_Generator_main) --> C([manage.py])


    LA(QR_Generator dummy):::hidden --> DB([asgi.py])
    LA(QR_Generator dummy):::hidden --> DC([settings.py])
    LA(QR_Generator dummy):::hidden --> DD([urls.py])
    LA(QR_Generator dummy):::hidden --> DE([wsgi.py])

    L --> LA

    KA(home_app dummy):::hidden --> KB(migrations)
    KA(home_app dummy):::hidden --> KC(Static Base)
    KA(home_app dummy):::hidden --> KD(templates/home)
    KA(home_app dummy):::hidden --> KE([apps.py])
    KA(home_app dummy):::hidden --> KF([urls.py])
    KA(home_app dummy):::hidden --> KG([utils.py])
    KA(home_app dummy):::hidden --> KH([views.py])

    KDA(home_app_htmls dummy):::hidden --> KDB([not_logined.html])
    KDA(home_app_htmls dummy):::hidden --> KDC([logined.html])

    KD --> KDA
    K --> KA


    JA(qrcode_app dummy):::hidden --> JB(migrations)
    JA(qrcode_app dummy):::hidden --> JC(Static Base)
    JA(qrcode_app dummy):::hidden --> JD(templates)
    JA(qrcode_app dummy):::hidden --> JE([admin.py])
    JA(qrcode_app dummy):::hidden --> JF([models.py])
    JA(qrcode_app dummy):::hidden --> JG([urls.py])
    JA(qrcode_app dummy):::hidden --> JH([views.py])

    JDA(qrcode_app_htmls dummy):::hidden --> JDB([active.html])
    JDA(qrcode_app_htmls dummy):::hidden --> JDC([my_qrcodes.html])
    JDA(qrcode_app_htmls dummy):::hidden --> JDD([generator_qr.html])

    JD --> JDA
    J --> JA


    IA(user_app dummy):::hidden --> IB(migrations)
    IA(user_app dummy):::hidden --> IC(Static Base)
    IA(user_app dummy):::hidden --> ID(templates)
    IA(user_app dummy):::hidden --> IE([admin.py])
    IA(user_app dummy):::hidden --> IF([models.py])
    IA(user_app dummy):::hidden --> IG([urls.py])
    IA(user_app dummy):::hidden --> IH([views.py])

    IDA(user_app_htmls dummy):::hidden --> IDB([confirm.html])
    IDA(user_app_htmls dummy):::hidden --> IDC([log.html])
    IDA(user_app_htmls dummy):::hidden --> IDD([reg.html])

    ID --> IDA
    I --> IA


    G(media) --> GA(images)
    GA(images) --> GB(qrcodes)
    GB(qrcodes) --> GC(User personal QR Codes)


    F(templates) --> FA([base.html])


    EY(Static Base) --> EYA(css)
    EY(Static Base) --> EYB(js)
    EY(Static Base) --> EYC(images)
    EY(Static Base) --> EYD(fonts)

    EYA(css) --> EYAA([style.css])
    EYB(js) --> EYBA([script.js])
    EYC(images) --> EYCA(any images for web page)
    EYD(fonts) --> EYDA(Only in global static app, fonts)

    classDef hidden display: none

```

</details>

## Структура додатку / Application structure

<details>

<summary>Натисніть, щоб побачити пояснення до структури додатків цього веб додатку / Click to see the explanations of the applications structure of this web application</summary>

*app - Папка у якій створен веб додаток і його базові складові (інші є у папці static та templates) / The folder in which the web application and its basic components are created (others are in the static and templates folder)

    admin.py - Відповідає за реєстрацію моделі для адмін сторінки (а також за її оформлення) / Responsible for registering the model for the page admin (as well as for its design)

    apps.py - Відповідає за головну інформацію додатку для роботи Django фреймворка / Responsible for the main information of the application for the Django framework to work

    models.py - Відповідає за моделі (таблиці) у базі даних / Responsible for models (tables) in the database

    tests.py - Відповідає за проведення серій тестів за допомогою Django інструментів (не використовується) / Responsible for running a series of tests using Django tools (not used)

    urls.py - Відповідає за встановлення посилання до сторінок, а також функцій, котрі їх оброблюють / Responsible for establishing links to pages, as well as the functions that process them

    templates - Папка у якій зберігаються усі веб сторінки даного додатку / Folder in which all web pages of this application are stored

        *.html - Відповідає за конструкцію веб сторінки / Responsible for the design of the web page


project - Папка, у якій створено всі складові фундаменту проекту / Folder in which all components of the foundation of the project are created

    asgi.py - Відповідає за асинхронну, складнішу, але більш швидку роботу Django (фреймворку, який відповідає за цілий бекенд) / Responsible for the asynchronous, more complex, but faster work of Django (the framework responsible for the entire backend)

    settings.py - Відповідає за налаштування роботи бекенду / Responsible for configuring the backend

    urls.py - Відповідає за налаштування веб адресів сторінок та media файлів / Responsible for setting web addresses of pages and media files

    wsgi.py - Відповідає за синхрону, простішу, але повільнішу роботу Django (фреймворк, який відповідає за цілий бекенд) / Responsible for the synchronous, simpler, but slower operation of Django (the framework responsible for the entire backend)


static - Папка у якій зберігаються усі статичні файли (js/css/картинки) / Folder in which all static files (js/css/images) are stored


    *_app - Папка яка відповідає за статичні файли вказаного додатка / The folder responsible for the static files of the specified application

        js - Папка, у якій зберігаються усі js скрипти / The folder where all js scripts are stored

            script.js - Файл з скриптом додатку / Application script file

        css - Папка, у якій зберігаються усі css стилі / The folder where all css styles are stored

            styles.css - Файл з стилями додатку / Application styles file

        images - Папка, у якій зберігаються усі зображення / The folder where all images are stored

        fonts - Папка, у якій зберігаються усі шрифти / The folder where all fonts are stored
            
            *.ttf - Файл з інформацією про шрифт / Font information file


manage.py - Файл, який користується для роботи вас з цим проектом / The file that you use to work with this project

README.md - Файл, котрий ви зараз читаєте. Створенний для пояснювання проекту для оточуючих. / The file you are currently reading. Created to explain the project to others. 
</details>

## Додатки / Applications

<details>

<summary>Натисніть, щоб побачити пояснення до додатків цього веб додатку / Click to see the explanations of the applications of this web application</summary>
<!-- TODO -->

### Home app (у коді просто home_app / in the code just home_app)
- Цей додаток відповідає за домашню сторінку, а саме за першу сторінку, що побачить користувач коли перейде на цей вебсайт / This application is responsible for the homepage, namely the first page that the user will see when they go to this website.
- Також, саме на сторінці, за яку відповідає цей додаток, користувач може оформити підписку / Also, it is on the page for which this application is responsible that the user can subscribe.

### Contacts app (у коді просто contacts_app / in the code it's just contacts_app)
- Цей додаток відповідає всього за одну сторінку, а саме за сторінку контактів / This application is responsible for only one page, namely the contacts page.
- Якщо ви хочете встановити свої контактні дані на сторінку, будь ласка, переглянте HTML шаблон у сторінці templates, та замініть потрібні посилання / If you want to set your contact details on the page, please review the HTML template in the templates page, and replace the necessary links.

### User app (у коді просто user_app)
- Цей додаток відповідає за всю роботу з системою користувачів, а також підписок / This application is responsible for all work with the user system, as well as subscriptions
- У цьому додатку є 2 сторінки - сторінка реєстрації та авторизації / This application has 2 pages - registration and authorization page
- Після реєстрації користувачу на пошту приходе повідомлення про підтвердження своєї пошти, тому одна пошта може бути тільки на один акаунт, так само як і логін / After registration, the user receives a confirmation message to their email, so one email can only be used for one account, as well as a login.
- Цей додаток містить дві моделі бази даних - Subscription та Account / This application contains two database models - Subscription and Account

### QRCode App (у коді просто qrcode_app / in the code just qrcode_app)
- Цей додаток відповідає за всю роботу з QR кодами, а саме їх створювання та управління / This application is responsible for all work with QR codes, namely their creation and management.
- При створенні QR коду, є можливість обрати колір, зображення та форму "квадратиків", докладніше у [Особливостях роботи додатків](#особливості-роботи-додатків--features-of-the-applications) / When creating a QR code, you can choose the color, image, and shape of the "squares", for more details see [Features of the applications](#особливості-роботи-додатків--features-of-the-applications)
- Всі свої QR коди користувач може побачити на сторінці My QR Codes, де він може їх завантажити або видалити с серверу, звільнивши собі місце під інший QR код. Коли його QR коди деактивовані, він може про це дізнатися по пункту Active у детальному перегляді QR коду або просто по затемненню QR коду. / The user can see all his QR codes on the My QR Codes page, where he can download or delete them from the server, freeing up space for another QR code. When his QR codes are deactivated, he can find out about it by clicking the Active item in the detailed view of the QR code or simply by darkening the QR code.
- Цей додаток містить одну модель бази даних - QRCode, яка має індивідуальний показ на сторінці адмінстрації, бо звичайний, котрий дає Django, не дуже зрозумілий / This application contains one database model - QRCode, which has an individual display on the administration page, because the regular one provided by Django is not very clear.

</details>

---

## Особливості роботи додатків / Features of the applications

<details>
<summary>Натисніть, щоб побачити додаткове пояснення по тому, як працює цей додаток / Click to see a further explanation of how this app works</summary>

### Підписки / Subscriptions

#### Підписку працюють місячно - при оформленні підписки активується таймер на 28 днів, котрий, коли завершується, автоматично переводе користувача на Free підписку, та деактивує ті QR коди які не входять в його новий план (Free) / Subscriptions are monthly - when subscribing, a 28-day timer is activated, which, when completed, automatically switches the user to a Free subscription and deactivates those QR codes that are not included in his new plan (Free)
#### Перевірка на те, чи закінчився QR код виконується кожний раз, коли користувач заходе на сайт, або користується QR кодом / A check to see if the QR code has expired is performed every time a user visits the site or uses the QR code.

### Генерація QR коду / QR code generation

#### Кожний QR код може мати кастомізовані / Any QR code can be customized in:
- Колір заднього фону (задній колір) / Background color (back color)
- Колір самого коду (передній колір) / The color of the code itself (front color)
- Зображення у центрі / Image in the center
- Форму квадратиків (пікселів, що складають QR код, не зображення) / The shape of the squares (the pixels that make up the QR code, not the image)
- Розмір квадратиків (може використовуватись для поліпшення якості зображення) / Square size (can be used to improve image quality)
#### Як це працює / How this works: 
- Для кольорів, використовується бібліотека qrcode (пояснення до котрої ви можете знайти у [Технологіях](#python)) / For colors, the qrcode library is used (an explanation of which you can find in [Technologies](#python))
- Для зображення в центрі, на зображення QR коду накладається зображення, котре вибере користувач, за допомогою бібліотеки [pillow](#python) / For the image in the center, the QR code image is overlaid with an image selected by the user using the [pillow](#python) library.
- Для форми та розміру квадратиків також використовується бібліотека qrcode / The qrcode library is also used for the shape and size of the squares.
</details>

---

## Посилання / Links

#### Посилання на проект у Figma, де створювався дизайн проекту / Link to the project in Figma where the project design was created: https://www.figma.com/design/QNoAIRnomVT5osDP8dU3UM/Home-Practice?node-id=134-177&t=FuI9B4tIHoOlSSk8-1
#### Посилання на план у Figma, де створювалися плани по праці учасників / Link to the plan in Figma, where plans were created for the participants' work: https://www.figma.com/board/P4KgGtiq4TJ3X0dHWhDJvY/Plan-Of-Work?node-id=0-1&t=JoM3sIPkIrwYYNwa-1
#### Посилання на структури бази даних у Figma / Link to database structure in Figma: https://www.figma.com/board/VpeI3GYLCqhbyMfpli80bX/Database-Schema?node-id=0-1&t=574WimiZcyrxKusN-1

---

## Висновок / Conslusion

### Цей додаток навчив нас просунутої роботі с багатьма аспектами роботи з широким фреймворком Django, а саме / This application taught us advanced work with many aspects of working with the broad Django framework, namely:
- Роботи з media файлами - як вони працюють, як їх оброблювати та правильному їх використанню / Working with media files - how they work, how to process them and their correct use
- Роботи статичних файлів (static) у Django, а саме їх підключення та різниця їх від других фреймворків, як, наприклад, Flask / How static files work in Django, namely their connection and their difference from other frameworks, such as Flask
- Структурі проекту Django - створення додатків та їх файлова структура / Django project structure - creating applications and their file structure
- Зручній та швидкій роботи з базою даних за допомогою Django / Convenient and fast database work with Django
### Про базу даних, ми використовували її, а не нереляційну базу даних, як от JSON, бо / About the database, we used it, not a non-relational database like JSON, because:
- Бази даних дозволяють швидкий та ефективний доступ к даним за потреби / Databases allow for quick and efficient access to data when needed
- Працюють відмінно при великих масштабах даних / Works great with large data scales
- Є набагато легшими для модерації, що дозволяє оперативно виправляти можливі помилки за потреби / They are much easier to moderate, allowing you to quickly correct possible errors if necessary.
#### Відходячи недалеко від теми, ми також вивчили (та використали) нові типи зв'язків, а саме / Going a little off topic, we also learned (and used) new types of connections, namely:
- Один до Одного - Використовували щоб поєднати користувача з системи з своєю моделлю профіля користувача, бо один користувач може мати тільки один профіль / One to One - Used to connect a user from the system to their user profile model, because one user can only have one profile
- Один до Багатьох - Використовували щоб поєднати користувача з його QR кодами, бо один користувач може мати багато QR кодів / One to Many - Used to associate a user with their QR codes, as one user can have many QR codes

### Також ми познайомились с новою для нас бібліотекою - qrcode / We also got acquainted with a new library for us - qrcode:
- Ми навчилися створювати різноманітні QR коди різної складності / We learned how to create various QR codes of varying complexity.
- Ми дізналися, як можна налаштовувати стилі QR кодів, як от їх колір, або фігуру / We learned how to customize QR code styles, such as their color or shape.
- Знайшли використання бібліотеці pillow в створенні QR кодів / Found use for the pillow library in creating QR codes

### Змогли значно покращити організацію команди за допомогою наступних інструментів / We were able to significantly improve team organization using the following tools:
#### Git - інструмент для розробки коду / Git - a tool for code development:
- Він дозволив відстежувати працю кожного учаснику команди за допомогою декількох кліків / It allowed tracking the work of each team member with just a few clicks.
- Допоміг нам коли були загублені частини коду, бо дозволяє доступ до минулих версій коду / Helped us when parts of the code were lost, because it allows access to past versions of the code
#### Figma - Інструмент для створення дизайну / Figma - Design creation tool:
- Ми навчилися створювати дизайни та робити для них прототипи, що поліпшує розуміння, як воно повинно виглядати у коді / We learned how to create designs and prototype them, which improves our understanding of how it should look in code.
- Краще зрозуміли як робити дизайн по макету з Figma / Better understand how to design from a mockup with Figma
#### FigJam - Інструмент для планувань та схем роботи / FigJam - A tool for planning and workflows:
- Познайомились з тим, що таке FigJam та використали для створень плану роботи / We got to know what FigJam is and used it to create a work plan.
- Полегшили розуміння бази даних, створивши її візуальну схему у FigJam / Made the database easier to understand by creating a visual diagram of it in FigJam  
<!-- TODO -->
