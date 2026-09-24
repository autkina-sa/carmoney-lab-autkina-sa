C:/Users/annac/carmoney-lab/carmoney-lab-autkina-sa/.kilo/worktrees/colossal-hair d4c5f38 [colossal-hair]
C:/Users/annac/carmoney-lab/carmoney-lab-autkina-sa/.kilo/worktrees/verbena-plant d4c5f38 (detached HEAD)

Тесты в `tests/Unit/`:

- `VinValidatorTest.php` — проверяет формат VIN (длина 17, регистр, запрещённые буквы I/O/Q, спецсимволы, пустая строка).
- `LtvCalculatorTest.php` — проверяет расчёт LTV в процентах и выброс `InvalidArgumentException` при нулевой оценочной стоимости и неположительной сумме.
- `DecisionEngineTest.php` — проверяет пороговое решение `approve` / `review` / `reject` по LTV на границах зон.
- `AssessmentServiceTest.php` — сквозная проверка сервиса оценки: LTV, решение, лимит и возраст ТС для низкого/среднего/высокого LTV.
- `ApplicationValidatorTest.php` — проверяет валидацию заявки: нормализация VIN, отказ при будущем годе, сумме ниже минимума и сбор всех ошибок сразу.

Работаю в `C:\Users\annac\carmoney-lab\carmoney-lab-autkina-sa\.kilo\worktrees\colossal-hair`, ветка `colossal-hair`.