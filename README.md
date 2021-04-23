# Types-and-structure
1. 
- Электронные чеки в json виде. Подойдёт NoSQL, т.к. позволяет хранить данные в json виде и в виде документов.
- Склады и автомобильные дороги для логистической компании. Подойдёт Реляционная база данных, структурированная БД.
- Генеалогические деревья. Иерархическая БД один родитель может иметь несколько детей.
- Кэш идентификаторов клиентов с ограниченным временем жизни для движка аутенфикации. Redis
- Отношения клиент-покупка для интернет-магазина. MongoDB позволяет вести данные комерции.

2.
CAP-теорема:
- Данные записываются на все узлы с задержкой до часа (асинхронная запись). Согласованность данных и доступность.
- При сетевых сбоях, система может разделиться на 2 раздельных кластера. Устойчивость к разделению и доступность.
- Система может не прислать корректный ответ или сбросить соединение. Системы CP и AP.

PACELC-теорема:
- Данные записываются на все узлы с задержкой до часа (асинхронная запись). Доступность, согласованность.
- При сетевых сбоях, система может разделиться на 2 раздельных кластера. Доступность, согласованность.
- Система может не прислать корректный ответ или сбросить соединение. Время, согласованность.

3. 
Могут ли в одной системе сочетаться принципы BASE и ACID? Почему?
Нет не могут, т.к. полностью противопоставляются друг другу.

4.
Какие минусы выбора Pub/Sub системы?

Redis Pub/Sub. Система сообщений. Может возникнуть проблема с очередностью получения сообщений.
