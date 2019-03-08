# selenium-hh-update

Маленький скрипт, выполняющий автоматическую публикацию резюме на сайте [hh].

## Конфигурация

Для работы требуется требуется редактировать переменные логина и пароля и выполнить скрипт:

```
python3 /path/to/config.py
```

А также установить следующие пакеты :

```sh
$ pip3 install selenium
$ yaourt geckodriver
```

## Установка

Для автоматического выполнения создать таск в [cron]

```sh
$ (crontab -l; echo "0 */4 * * * python /path/to/config.py" ) | crontab
```

[cron]: http://help.ubuntu.ru/wiki/cron
[hh]: http://hh.ru
