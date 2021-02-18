# Django-base

Базовый шаблон Django проекта, с которого можно начать разработку. Сюда входит конфиг Systemd, nginx, gunicorn.

Установка представляет собой просто указание Python интерпретатора и названия домена, запустите:

```
./install.sh
```

В конфиге Django заполните настройки базы данных (`src/config/settings.py`)

Посмотреть статус gunicorn демона:

```
sudo systemctl status gunicorn
```

Логи gunicorn лежат в `gunicorn/access.log` и `gunicorn/error.log`

После изменения systemd конфига надо перечитать его и затем перезапустить юнит:

```
sudo systemctl daemon-reload
sudo systemctl restart gunicorn
```
https://vk.com/flaiers

https://t.me/flaiers
