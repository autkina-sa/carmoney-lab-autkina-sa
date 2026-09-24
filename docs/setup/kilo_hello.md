# kilo_hello

готов
1) Сервис (README.md:1-10): учебный carmoney-lab — предварительная оценка заявки на заём под ПТС, считает LTV и возвращает approve/review/reject, все данные синтетические.
2) Команды: Makefile — `make up|down|test|lint|seed|logs|ps|install|help` (Makefile:11-52); docker-compose.yml — сервисы `backend` (php -S 0.0.0.0:8080, порт ${APP_PORT:-8080}:8080) и `db` (mysql:8.0, порт ${DB_PORT:-3307}:3306, том db-data, init из db/schema.sql и db/seed.sql) (docker-compose.yml:1-45).
3) Решение approve/review/reject считается в `backend/src/Domain/` — DecisionEngine.php, LtvCalculator.php, AssessmentService.php (правила из backend/config/rules.php).

модель: MiniMax-M3
