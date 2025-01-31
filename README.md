# Обновление товаров Ozon и Яндекс Маркет

Данный скрипт автоматизирует работу с товарами. Он получает актуальные данные и изменяет их у товара.

## Что делает скрипт?
- Получает список товаров

- Получает данные об остатках и ценах от поставщика

- Обновляет данные: наличие на складе и цены

## Как пользоваться?

### Для Ozon:
1. Подключиться к Ozon через API ключ

2. Загрузить файл с остатками и ценами

3. Запустить скрипт

### Для Яндекс Маркета:
1. Подключиться к Яндекс Маркету через API ключ

2. Загрузить файл с остатками и ценами

3. Запустить скрипт

## Возможные ошибки

- "Превышено время ожидания..." 

- "Ошибка соединения" 

- "ERROR_2" 

## Переменные окружения

### Для Ozon:
Для работы скрипта нужен ключ доступа API. Получить его можно тут (https://seller.ozon.ru/app/registration/signin?redirect=L3NldHRpbmdzL2FwaS1rZXlz):

Данные нужно сохранять в файле формата '.env':
```
SELLER_TOKEN = 'api ключ'
CLIENT_ID = 'идентификатор магазина'
```

### Для Яндекс:
Для работы скрипта нужен ключ доступа API. Получить его можно тут (https://yandex.ru/dev/market/partner-api/doc/ru/concepts/api-key):

Данные нужно сохранять в файле формата '.env':
```
MARKET_TOKEN = 'api ключ'
CLIENT_ID = 'идентификатор магазина'
FBS_ID = 'идентификатор FBS'
DBS_ID = 'идентификатор DBS'
WAREHOUSE_FBS_ID = 'идентификатор склада FBS'
WAREHOUSE_DBS_ID = 'идентификатор склада DBS'
```

## Код для запуска:
```
python 'название скрипта'.py
```