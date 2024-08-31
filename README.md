<b>Крок 1: Запуск першого контейнера Docker</b>

<a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/1.1.png" >Команда  docker run -d -p 8080:80 docker/welcome-to-docker</a> завантажує образ Docker і запускає контейнер з публікацією порту 80 контейнера на порт 8080 хоста. Після виконання цієї команди, контейнер запущено і інтерфейс доступний через <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/1.2.png">http: //localhost:8080.</a> 

<b>Крок 2: Клонування та запуск проекту</b>

<a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/2.1.png">Команда git clone</a> виконує клонування проекту, а <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/2.2.png">команда docker compose watch </a> запускає середовище розробки з використанням Docker Compose.
Після запуску проекту додаток стає доступним за адресою <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/2.3.png">http: //localhost.</a> На сторінці відображається проста програма для ведення списку завдань.

<b>Крок 3: Внесення змін у додаток</b>

Внесено кілька змін до додатка: текст привітання був змінений у файлі <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/2.4.png">backend/src/routes/getGreeting.js</a>, щоб відображати випадкове привітання з масиву. Текст у формі додавання нового елемента був змінений у файлі <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/2.5.png">client/src/components/AddNewItemForm.jsx</a>. А також в <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/2.6.png">client/src/index.scss</a> змінено колір фону. Після внесення цих змін можна одразу побачити <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/2.7.png">результат</a> в реальному часі без необхідності перезапуску.

<b>Крок 4: Створення Docker зображень</b>

<a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/3.1.png">Команда docker build</a> використовується для створення Docker зображення з проекту. Після виконання команди, зображення можна перевірити за допомогою <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/3.2.png">docker image ls</a>.

<b>Крок 5: Завантаження Docker зображень</b>

<a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/3.3.png">Команда docker push</a> використовується для відправки створеного Docker зображення до Docker Hub. Після виконання команди, <a href="https://github.com/Anastassssssia/Docker_Ivanchoglo_Anastasia/blob/09604199cdba18063d671a0b678fdc783bd2f940/screenshots/3.4.png">зображення</a> стає доступним у створеному сховищі на Docker Hub для подальшого використання або завантаження іншими користувачами.
