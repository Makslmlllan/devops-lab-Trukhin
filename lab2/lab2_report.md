# Лабораторная работа №2  
## CI/CD для Docker приложения

### Цель работы
Настроить CI/CD pipeline для автоматической сборки Docker образа и публикации его в Docker Hub.

---

### Ход работы

1. В репозиторий были добавлены файлы приложения:
- app.py
- requirements.txt
- Dockerfile

2. Был создан Docker Hub репозиторий:

makslmlllan/my-flask-app

3. В GitHub была создана директория:

.github/workflows

4. Создан pipeline файл:

docker-build.yml

Pipeline выполняет следующие шаги:
- checkout репозитория
- настройка Docker Buildx
- login в Docker Hub
- сборка Docker образа
- push образа в Docker Hub

5. В GitHub Secrets были добавлены переменные:

DOCKER_USERNAME  
DOCKER_PASSWORD

6. После выполнения pipeline Docker образ был успешно загружен в Docker Hub.

---

### Результат

CI/CD pipeline автоматически собирает Docker образ и публикует его в Docker Hub при каждом push в ветку main.
