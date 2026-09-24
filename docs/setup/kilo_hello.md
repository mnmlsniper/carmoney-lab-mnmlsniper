# Ответ на задание 1.1.3

готов

1) Сервис: предварительная оценка заявки на заём под ПТС — принимает заявку, считает LTV и возвращает решение approve / review / reject (учебный проект, все данные синтетические).
2) Makefile: `make up` (поднять сервис и базу, http://localhost:8080), `make down`, `make ps`, `make logs`, `make install`, `make test` (PHPUnit), `make lint` (php -l), `make seed`; docker-compose.yml — сервисы backend (PHP 8.3 + Slim, порт ${APP_PORT:-8080}) и db (MySQL 8.0, порт ${DB_PORT:-3307}), команды запуска там нет.
3) Решение approve / review / reject считается в `backend/src/Domain/` (класс DecisionEngine.php).

модель: training-2026-09-glm-5.3
