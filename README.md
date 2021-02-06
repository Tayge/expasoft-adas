<h1>Expasoft-ADAS</h1>
Проект Expasoft ADAS на Зимней Школе CompTech 2021
<h2>Описание</h2>
ADAS (Advanced Driver Assistance Systems) – интеллектуальные системы помощи водителям автомобилей. Основная функция таких систем – повышение безопасности эксплуатации транспортных средств, которое способствует глобальному снижению уровня ДТП на дорогах.<br>
Даже самые простые функции, такие как звуковые сигналы или голосовые сообщения при приближении к препятствию, «потере» своей полосы, а также приближению к пешеходам, повышают концентрацию водителя и мотивировать его снизить скорость или совершить определенный маневр. <br>
В репозитории находится прототип приложения, которое должно предупреждать водителей об опасных ситуациях. <br>
<h2>Цель</h2>
Прототип должен отслеживать пешеходов, дорожную полосу и знаки дорожного движения<br>

<h2>Содержание</h2>
Models - натренированные модели<br>
nootebooks - Рабочие ноутбуки команды <br>

<h2>Пример использования сегментации</h2>
https://youtu.be/S3bjPXZyq_c

<h2>Архитектура </h2>
Сегментация осуществляется с помощью нейронной сети Unet с энкодером efficientnet-b0, на базе API Segmentation Models Pytorch. Сеть была натренирована на датасете BDD100K. <br>
За классификацию дорожных знаков отвечает MobileNet V2 натренированная на изображениях российских дорожных знаков.<br>
Детекцию автомобилей, пешеходов и дорожных знаков "осуществляла" MobileNetV2-SSD, натренированная на датасете BDD100K.<br>
