В составе два приложения wordpress и monitorings
- Для запуска необходимо находясь в каталоке арр в файлом Makefile ввести в терминале команду:
make up       - запускает все сервисы
make down     - останавливает все сервисы
make restart  - перезапускает все сервисы
make up-app   - запускает отдельно приложение wordpress
male up-mon   - запускает отдельно приложение мониторинга

============WORDPRESS============

- В браузере перейти по адресу:
localhost

- Заполнить форму с необходимыми параметрами:
Язык - Русский 
login: test
password: test
Разрешить использование слабого пароля.
e-mail: test@example.com

Для активации ObjectCaches
Перейти в раздел плагины
Активировать плагин Redis Object Cache
Нажать Enable Object Cache

============MONITORING============

Для доступа к панели мониторинга
В браузере перейти по сслыке
localhost:3000

login: admin
password: admin

пропустить установку пароля кнопкой skip

В левой панели зайти в Dashboards далее открыть каталог All dashboards и выбрать интересующую 
панель

Node Exporter Full         - отображдает информацию о нагрузке на хост систему
cAdvisor Docker Insights   - состояние контенеров (временно не работает)
Logs / App                 - информация о логах (временно не работает)