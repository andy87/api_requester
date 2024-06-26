
# Полный список изменений.

## 99b
24/05/2024 (Глобальная переработка + Покрытие тестами)
- Добавления:
  - `knockKnock`
    - добавлены readonly свойства
    - Новые методы:
      - useCookie()
      - enableRedirect()
      - validateHostName()
    - Новые события:
      - EVENT_CURL_HANDLER
  - `Response`
    - добавлены readonly свойства
    - Новые методы:
      - asArray()
      - validate()
  - `Request`
    - добавлены readonly свойства

- Изменения:
  - `knockKnock`:
    - переделаны setter & getter
    - disableSSL()
    - enableSSL()
  - `Request`:
    - переделаны setter & getter
    - disableSSL() - теперь может принимать аргументы
    - enableSSL() - теперь может принимать аргументы
  - `Response`:
    - переделаны setter & getter
    - __construct() - $request стал обязательным
    - getErrors() - теперь возвращает массив собственных ошибок
    - get() - удалено

### 1.0.1
   - Исправлены ошибки в документации
   - Исправлены ошибки в коде
   - Исправлены ошибки в тестах

### 1.0.2
 - Изменения:
   - Переименование:
     - `KnockKnock` -> `Operator`
     - `KnockRequest` -> `Request`
     - `KnockResponse` -> `Response`
   - Упрощена логика(схема) работы
   - Переформатирован код:
     - Code Style ближе к PSR-4
     - сгруппированы методы и свойства
   - Operator:
     - send() - теперь принимает `$request` вместо `$fakeResponse`
 - Добавлено:
   - add `github/workflows` for CI/CD
   - Autoloader
   - `Exception` на многие случаи
   - Request
     - добавлен метод `setFakeResponse`
     - добавлено ReadOnly свойство `$fakeResponse`

### 1.2.1
 - Мелкие правки
 - Добавлены тесты

### 1.3.0
 - fix packagist
 - 
### 1.3.1
 - codeStyle
 - fix test

### 1.3.2
- codeStyle
  - add comments Exception
- update README
- setup: "minimum-stability": "dev",