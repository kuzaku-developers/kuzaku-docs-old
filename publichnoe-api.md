# Публичное API

**API** предоставляет Вам возможность взаимодействовать с ботом за пределами наших официальных сервисов. Ниже Вы найдете небольшую справку, которая будет описывать задачу каждого эндпоинта.

Стоить приметить, что на текущий момент API находится в разработке. Поэтому, существует только **2** публичных эндпоинта, которые может использовать каждый. В будущем возможности API будут значительно расширятся.

## Методы

{% api-method method="get" host="https://kuzaku.ml/api" path="/v1/statistic/" %}
{% api-method-summary %}
Получить статистику бота
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
ответ в случае успеха.
{% endapi-method-response-example-description %}

```
{"status":"200", "message":"all is ok", "guilds":"666", "users":"6666"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
ответ если метод не найден.
{% endapi-method-response-example-description %}

```
{"status":"404", "message":"method not found"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=503 %}
{% api-method-response-example-description %}
ответ если бот оффлайн.
{% endapi-method-response-example-description %}

```
{"code":"503","message":"bot is offline!"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



{% api-method method="get" host="https://kuzaku.ml/api" path="/v1/ping/" %}
{% api-method-summary %}
Пингануть бота
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{"status":"200", "message":"all is ok"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{"status":"404", "message":"method not found"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=503 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{"code":"503","message":"bot is offline!"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

