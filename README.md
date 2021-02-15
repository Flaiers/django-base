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

![Photo](https://i.ibb.co/kSFbhZs/IHDqc-V-2-GI-u-Ku-WXpo-Qc-D5uerr-A5-Gi-Wm-Zw-Fji-JVSx-Xi-RTl-E4d-E7f-AGHqwd-P0m-Wa4-Bi-IYHSr1-bt-l-W.jpg)
