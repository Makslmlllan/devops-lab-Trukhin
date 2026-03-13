Lab 3 — Мониторинг с Prometheus и Grafana

Цель работы
Развернуть систему мониторинга с использованием Prometheus, Node Exporter и Grafana.

Используемые инструменты
- Docker
- Prometheus
- Grafana
- Node Exporter

Ход работы

1. Создан docker-compose файл для запуска сервисов:
Prometheus
Grafana
Node Exporter

2. Настроен Prometheus для сбора метрик

3. Grafana подключена к Prometheus как источник

4. Создан dashboard для мониторинга 

Добавлены следующие графики:

RAM usage
Disk usage и GPU 

Результат

Создан дашборд Grafana для мониторинга ресурсов
