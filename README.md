установить на него PostgreSQL 13 с дефолтными настройками
--![image](https://user-images.githubusercontent.com/45406197/182200335-ca22768b-dcaa-4e68-beed-062836337e47.png)

применить параметры настройки PostgreSQL из прикрепленного к материалам занятия файла
выполнить pgbench -i postgres
--![image](https://user-images.githubusercontent.com/45406197/182200541-9b1219c0-431b-498f-9d81-0addb7023ebb.png)

запустить pgbench -c8 -P 60 -T 3600 -U postgres postgres
дать отработать до конца
зафиксировать среднее значение tps в последней ⅙ части работы
а дальше настроить autovacuum максимально эффективно
так чтобы получить максимально ровное значение tps на горизонте часа
