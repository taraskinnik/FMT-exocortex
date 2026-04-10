# IWE Agent Entry Point

Этот файл — compatibility entrypoint для AI-агентов, которые ищут `AGENTS.md`.

## Что читать сначала

1. `CLAUDE.md` — source-of-truth по операционным правилам IWE.
2. `memory/protocol-open.md`, `memory/protocol-work.md`, `memory/protocol-close.md` — полный ОРЗ-фрактал.
3. `params.yaml` — пользовательские параметры, включая выбранный `agent_id`.

## Базовые правила для любого агента

- Рабочий язык — русский. EN только для кода, имён файлов, терминов и ключей YAML/JSON.
- Перед началом задачи проверяй актуальный план и соблюдай WP Gate.
- На рубежах работы делай `Capture-to-Pack`: если найдено устойчивое знание, явно предлагай, куда его зафиксировать.
- Не редактируй платформенные протоколы и skills напрямую, если `author_mode: false` — кастомизация идёт через `extensions/`.
- Экзокортекс — это экзоскелет, не автопилот: человек принимает стратегические и Pack-решения.

## Agent-specific layers

- Claude Code: `.claude/`, `CLAUDE.md`, `memory/`
- GitHub Copilot: `.github/copilot-instructions.md`, `AGENTS.md`, `memory/`
- Cursor: `.cursor/rules/iwe.mdc`, `AGENTS.md`, `memory/`
- Antigravity: `AGENTS.md`, `memory/`

## Минимальный стартовый workflow

1. Открой рабочую директорию `{{WORKSPACE_DIR}}`.
2. Прочитай `CLAUDE.md` и `memory/`.
3. Начни с фразы: «Проведём первую стратегическую сессию».
