# hotel-booking-test
# Hotel Booking API Tests

## Описание проекта

Этот проект включает в себя автоматизацию тестирования API сервиса бронирования отелей.

## Технологии

- Python
- pytest
- requests

## Инструкция по запуску

1. Клонируйте репозиторий:
    ```bash
    git clone https://github.com/yourusername/hotel-booking-tests.git
    cd hotel-booking-tests
    ```
2. Перейдите в директорию проекта и установите зависимости:
    ```bash
    python -m venv venv
    source venv/bin/activate  # Linux/Mac
    venv\Scripts\activate     # Windows
    pip install -r requirements.txt
    ```
3. Запустите тесты:
    ```bash
    pytest
    ```

## Тесты

- **Auth**
  - `test_auth_success`: Проверка успешной аутентификации.
  - `test_auth_failure`: Проверка ошибки при аутентификации с некорректными данными.

- **Booking - CreateBooking**
  - `test_create_booking_success`: Проверка успешного создания бронирования.
  - `test_create_booking_failure`: Проверка ошибки при создании бронирования с некорректными данными.

- **Booking - GetBooking**
  - `test_get_booking_success`: Проверка успешного получения информации о бронировании.
  - `test_get_booking_failure`: Проверка ошибки при запросе несуществующего бронирования.
