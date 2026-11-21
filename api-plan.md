# План API сервиса бронирования

## Авторизация
- POST /auth/register — регистрация по телефону
- POST /auth/login — выдача JWT

## Клубы и места
- GET /clubs/{id}/map — карта зала со статусами мест
- GET /clubs/{id}/tariffs — тарифы

## Бронирования
- POST /bookings — создать бронь
- POST /bookings/{id}/extend — продлить сессию
- POST /bookings/{id}/cancel — отменить

## Кошелёк
- GET /wallet — баланс
- POST /wallet/topup — пополнение  

## Real-time (WebSocket)
- WS /realtime/map — live-обновление статусов мест для админки
- WS /realtime/session — тикание таймера сессии у игрока