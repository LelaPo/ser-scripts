[![version](https://img.shields.io/badge/ser-v1.0.0-black?style=flat-square)](https://github.com/ScriptedEvents/ScriptedEventsReloaded)
[![license](https://img.shields.io/github/license/LelaPo/ser-scripts?style=flat-square)](LICENSE)

# ser-scripts

небольшой набор готовых скриптов для scripted events reloaded (scp:sl).
адаптировано под ser 1.0.0, с чистым синтаксисом, плавной cassie на русском и встроенными командами для тестов.

## что внутри

* **`scripts/customCoin.ser`** — хаотичная монетка при подбрасывании. умеет телепортировать (к scp, на улицу или в боеголовку), выдавать редкие конфеты, отрубать руки, выбивать/блокировать двери или спавнить гранаты. подробнее в [docs/customCoin.md](docs/customCoin.md).
* **`scripts/scp3114.ser`** — спавн скелета в начале раунда с шансом 15%. аккуратно заменяет случайного scp (кроме 079) и запускает студийное оповещение cassie с синхронными русскими субтитрами. подробнее в [docs/scp3114.md](docs/scp3114.md).

## как установить

1. скопируй нужные `.ser` файлы в директорию:
   `LabAPI/configs/Scripted Events Reloaded/`
2. в консоли сервера напиши `serreload` (или начни новый раунд).

## команды для проверки

можно вводить прямо в игровой консоли на `~` или в remote admin:

* `.scp3114` — превращает тебя в скелета и проигрывает cassie
* `.scp3114 random` — симулирует выбор случайного scp из раунда
* `.testcoin <число или слово>` — моментально запускает любой исход монетки (например, `.testcoin tp`, `.testcoin jackpot`, `.testcoin pink`)
* `.testcoin doors <1-4>` — проверка действий с дверями (1 — открыть, 2 — запереть, 3 — сломать, 4 — рандом)

## документация

* `docs/` — подробные описания скриптов, шансы выпадения и параметры команд.
* `Documentation/` — справочники методов, свойств, типов предметов и ивентов ser 1.0.0, а также примеры скриптов.

## лицензия

[mit](LICENSE)