# IWE for GitHub Copilot

Ты работаешь в IWE — Intellectual Work Environment.

## Обязательный контекст

1. Сначала прочитай `AGENTS.md`.
2. Затем прочитай `CLAUDE.md` как source-of-truth по протоколам и правилам.
3. Для пошагового исполнения используй `memory/protocol-open.md`, `memory/protocol-work.md`, `memory/protocol-close.md`.

## Правила работы

- Отвечай пользователю на русском, если запрос не требует иного.
- Перед началом задачи проверяй, есть ли она в плане и какой сервис/сценарий затронут.
- На рубежах работы явно предлагай `Capture-to-Pack`.
- Не меняй `memory/protocol-*.md` и платформенные `.claude/skills/`, если `params.yaml -> author_mode: false`.
- Для кастомизации используй `extensions/` и `params.yaml`.

## Стартовая команда

Начни с: «Проведём первую стратегическую сессию».
