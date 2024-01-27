# django_api
Для запуска
1) git clone https://github.com/yzajchenko/django_api.git
2) docker-compose up
Разрешения имеют толькот авторизованные пользователи

Для доступа нужно авторизоваться:

1) Зарегистрироваться отправив post запросом http://0.0.0.0:8001/auth/users/ name, password, email
2) Авторизоваться отправив post запросом http://0.0.0.0:8001/auth/token/login/ name, password, в ответ получим token, который отправляется в заголовках запроса
Key: Authorization
Value: Token "you token"

Создания Category отправить post запрпос http://0.0.0.0:8001/api/category/
Просмотр Category отправить get запрос http://0.0.0.0:8001/api/category/
Для просмотра Category по id get запрос http://0.0.0.0:8001/api/category/id/
Для обновления Category put запрос http://0.0.0.0:8001/api/category/id/
Удаления Category DELETE запрос http://0.0.0.0:8001/api/category/id/

Создания Priority отправить post запрпос http://0.0.0.0:8001/api/priority/
Просмотр Priority отправить get запрос http://0.0.0.0:8001/api/priority/
Для просмотра Priority по id get запрос http://0.0.0.0:8001/api/priority/id/
Для обновления Priority put запрос http://0.0.0.0:8001/api/priority/id/
Удаления Priority DELETE запрос http://0.0.0.0:8001/api/priority/id/

Создания Task отправить post запрпос http://0.0.0.0:8001/api/tasks/
Просмотр всех Tasks отправить get запрос http://0.0.0.0:8001/api/tasks/
Просмотр всех Tasks по id or status отправить get запрос http://0.0.0.0:8001/api/tasks/?status=status
Для просмотра Task по id get запрос http://0.0.0.0:8001/api/task/id/
Для обновления Task put запрос http://0.0.0.0:8001/api/task/id/
Удаления Priority Task запрос http://0.0.0.0:8001/api/task/id/

Пользователи могут просматривать и обновлять только свои задачи
Категории созданные другими пользователями доступны только для чтения
Приоритеты созданные другими пользователями доступны только для чтения









