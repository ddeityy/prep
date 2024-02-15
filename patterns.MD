# Паттерны

## Порождающие паттерны
    Беспокоятся о гибком создании объектов без внесения в программу лишних зависимостей.
### Фабрика

### Абстрактная Фабрика

### Строитель

### Прототив

### Singleton

## Структурные паттерны
    Показывают различные способы построения связей между объектами.
### Adapter

### Bridge

### Composite

### Decorator

### Facade

### Flyweight

### Proxy

## Поведенческие паттерны
    Заботятся об эффективной коммуникации между объектами.
### Chain of Responsibility

### Command

### Iterator

### Mediator

### Memento

### Observer

### State

### Strategy

### Visitor

### Template

## Отказоустойчивые паттерны
    * Сокращение времени простоя сервисов.
    * Лучшая изоляция от сбоев.
    * Повышение производительности системы.
    * Повышение удовлетворенности пользователей.

### Circuit Breaker
    * Закрыт - все реквесты проходят
    * Открыт - все реквесты дропаются
    * Полуоткрыт - после "таймаута сброса" проходит фиксированное кол-во реквестов
        для теста восстановления.
        Если всё хорошо - переход в закрытое состояние.

### Bulkhead

### Timeout & Retry

### Rate Limiter
    Паттерн отказоустойчивости в распределенных системах
    предназначенный для защиты сервисов от чрезмерной нагрузки
    путем контроля скорости поступления запросов.

    Стратегии:
        * Фиксированное окно:
            x requests per hour (12:00 - 13:00) per client/IP
        * Скользящее окно
            x requests per hour (old vs new timestamp) per client/IP
        * Token Bucket
            global bucket with x tokens
            1 request = 1 token
            tokens slowly refill automatically
            no tokens = request dropped
        * Leaky Bucket
            global bucket with x requests
            requests are accepted at a fixed rate
            new request overfills the bucket = drop
            
### Fallback

### Health Check
