# awesome_project
Проект по прогнозированию объемов продаж топлива

Документация проекта: https://confluence/pages/123456432

## Инструкции по развертыванию приложения:
> Протестировано на Ubuntu 22.04 с предустановленным гитом и питоном

1. Клонировать репозиторий.
   Необходимо [сгенерировать токен](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)
   для возможности клонирования, пароль от аккаунта не подойдет (такая возможность была исключена)
```
git clone https://{token}@github.com/TrybinD/awesome_project.git
```

2. Установить make
```   
apt update && apt install make
```

3. Установить пакеты, запустить стримлит. Все инструкции написаны в makefile
```
make deploy
```

5. Для добавления данных, в том числе кеша на VPS необходимо с локальной машины скопировать папку data на VPS:
```
scp -r data root@185.46.11.220:/root/range_candidates
```
