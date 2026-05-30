# demoblaze-api-testing
## О проекте
Проект по тестированию API интернет-магазина Demoblaze с использованием Postman.

## Используемые инструменты
- Postman
- DevTools
- JSON
- GitHub

## Протестированные endpoints

### Login API
- Успешная авторизация
- Неверный логин и пароль
- Пустой password
- Пустой request body

### Product API
- Получение списка товаров
- Получение товара по валидному ID
- Проверка невалидного ID
- Проверка строкового значения вместо ID
- Проверка отсутствующего поля `id`
## Найденные проблемы

### Неверные status codes
- API возвращает `200 OK` при неверных credentials вместо `401 Unauthorized`
- API возвращает `200 OK` при validation errors вместо `400 Bad Request`

### Ошибки валидации
- API возвращает `500 Internal Server Error` при строковом значении ID

## Что проверялось
- Positive testing
- Negative testing
- Input validation
- Status codes
- Error handling
- JSON response validation


## Test Coverage

- Valid Login
- Invalid Login
- Empty Password
- Empty Request Body
- Product List Retrieval
- Product Details by Valid ID
- Product Details by Invalid ID
- Product Details by String ID
- Product Details with Missing ID

## Automated Checks

- Status Code Validation
- Response Time Validation
- Response Body Validation
- Error Message Validation
- Data Type Validation
- JSON Structure Validation
- Array Validation

## Results

- Requests: 9
- Automated Tests: 25
- Passed: 25
- Failed: 0
## Файлы проекта
- Postman Collection
- Automated API Tests
- Validation Scenarios
- Negative Test Cases
