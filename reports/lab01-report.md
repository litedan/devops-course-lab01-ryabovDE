# Отчёт по лабораторной работе №1
## Настройка локального окружения разработчика

**Студент:** Рябов Даниил Евгеньевич
**Группа:** 23-ИСбо-2
**Дата:** 2026-09-12

---

## 1. Информация о системе

### 1.1. Версия ОС
Distributor ID: Ubuntu
Description: Ubuntu 22.04.5 LTS
Release: 22.04
Codename: jammy


### 1.2. Версия ядра Linux
5.15.153.1-microsoft-standard-WSL2


## 2. Установленные инструменты

| Инструмент | Версия |
|---|---|
| Git | 2.34.1 |
| Docker | 27.3.1 |
| Docker Compose | v2.29.7 |
| Make | GNU Make 4.3 |
| curl | 7.81.0 |
| jq | jq-1.6 |
| kubectl | v1.31.1 |
| Helm | v3.16.2 |

## 3. Настройка Git

### 3.1. Конфигурация Git
user.name=daniil
user.email=daniilryabov1706@gmail.com
init.defaultbranch=main
core.autocrlf=input
core.editor=nano
pull.rebase=true
fetch.prune=true
alias.st=status
alias.co=checkout
alias.br=branch
alias.ci=commit
alias.lg=log --graph --oneline --decorate --all

## 4. SSH-ключ

### 4.1. Проверка подключения к GitHub
Hi daniilryabov1706! You've successfully authenticated, but GitHub does not provide shell access.

### 4.2. Отпечаток ключа
256 SHA256:LCqR/1IhFThTnVt88Y+G81TNqFKfSaPrEJo8YUF9Bok daniilryabov1706@gmail.com (ED25519)

## 5. Проверка Docker

### 5.1. Запуск hello-world
Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:

The Docker client contacted the Docker daemon.

The Docker daemon pulled the "hello-world" image from the Docker Hub.

The Docker daemon created a new container from that image which runs the
executable that produces the output you are currently reading.

The Docker daemon streamed that output to the Docker client, which sent it
to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
$ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
https://hub.docker.com/

For more examples and ideas, visit:
https://docs.docker.com/get-started/

## 6. Выводы
В ходе лабораторной работы было подготовлено локальное окружение разработчика на базе WSL2 с дистрибутивом Ubuntu 22.04. Установлен полный набор CLI-инструментов, необходимых для дальнейших работ курса: Git, Docker Engine, Docker Compose, Make, curl, jq, kubectl и Helm. Сгенерирован SSH-ключ по алгоритму Ed25519 и настроена аутентификация с GitHub — команда `ssh -T git@github.com` подтверждает успешное подключение. Выполнена настройка Git (имя, email, редактор, алиасы, поведение pull/fetch). Проверка работоспособности Docker через `docker run --rm hello-world` прошла успешно.

EOF
