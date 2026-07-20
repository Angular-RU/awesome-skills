<div align="center">

# Awesome AI Skills

**Курируемая коллекция Agent Skills для Claude Code, Codex, Gemini CLI, GitHub Copilot, Cursor и других AI-агентов.**

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

</div>

Agent Skills превращают повторяемые инструкции, знания и автоматизацию в переносимые модули, которые AI-агент может подключать по мере необходимости. Один и тот же skill можно использовать в разных проектах и, если он следует открытому формату, в разных AI-инструментах.

> **Последняя проверка списка:** 20 июля 2026 года. Популярность учитывается, но не является единственным критерием: также важны практическая польза, документация, лицензия и активность проекта.

## Содержание

- [Что такое Agent Skills](#что-такое-agent-skills)
- [Как установить skill](#как-установить-skill)
- [Каталог](#каталог)
- [Как устроен skill](#как-устроен-skill)
- [Как создать свой skill](#как-создать-свой-skill)
- [Как добавить проект в список](#как-добавить-проект-в-список)
- [Безопасность](#безопасность)

## Что такое Agent Skills

**Agent Skill** — это папка с инструкциями, скриптами и вспомогательными материалами, которая обучает AI-агента выполнять конкретную задачу или рабочий процесс.

Обычно агент сначала видит только имя и краткое описание skill. Полные инструкции загружаются, когда задача действительно подходит под его назначение. Такой подход называют **progressive disclosure**: контекст не переполняется всеми инструкциями сразу.

Skills подходят для:

- code review, отладки, тестирования и работы с Git;
- архитектурных и командных процессов;
- frontend, backend, DevOps, cloud и data-задач;
- подготовки документов, исследований и контента;
- хранения внутренних правил и знаний проекта.

### Skill и MCP — не одно и то же

- **Skill** объясняет агенту, **как** выполнять задачу: шаги, ограничения, примеры и проверки.
- **MCP** предоставляет агенту инструменты и данные во время выполнения: API, файловые системы, базы данных и внешние сервисы.

Они хорошо дополняют друг друга: MCP дает возможности, а skill задает надежный способ их использовать.

## Как установить skill

Многие современные репозитории поддерживают универсальный CLI [`skills`](https://github.com/vercel-labs/skills):

```bash
# Посмотреть доступные skills
npx skills add owner/repository --list

# Установить выбранный skill в текущий проект
npx skills add owner/repository --skill skill-name

# Установить глобально для всех проектов
npx skills add owner/repository --skill skill-name -g
```

Пример:

```bash
npx skills add vercel-labs/agent-skills --list
npx skills add vercel-labs/agent-skills --skill web-design-guidelines
```

| Режим | Когда использовать |
| --- | --- |
| **Project-local** | Skill должен храниться вместе с репозиторием и быть одинаковым у всей команды. |
| **Global** | Skill нужен лично вам во многих несвязанных проектах. |

Не все проекты используют одинаковый способ установки. Перед установкой проверяйте README конкретного репозитория: некоторые skills распространяются через Claude Code Marketplace, встроенный установщик Codex, собственный CLI или ручное копирование папки.

## Каталог

### Стандарт и официальные коллекции

| Репозиторий | Для чего нужен |
| --- | --- |
| [agentskills/agentskills](https://github.com/agentskills/agentskills) | Открытая спецификация Agent Skills, документация и правила совместимости. |
| [anthropics/skills](https://github.com/anthropics/skills) | Официальные примеры Anthropic: документы, таблицы, PDF, презентации, дизайн и технические workflows. |
| [openai/skills](https://github.com/openai/skills) | Официальный каталог skills для Codex с системными, курируемыми и экспериментальными наборами. |
| [google/skills](https://github.com/google/skills) | Официальные skills для Google Cloud, Gemini API, Firebase, BigQuery, Cloud Run, GKE и архитектурных практик. |
| [microsoft/skills](https://github.com/microsoft/skills) | Skills, custom agents и MCP-конфигурации для Azure SDK, Microsoft Foundry и облачной разработки. |
| [huggingface/skills](https://github.com/huggingface/skills) | Работа с Hugging Face Hub, датасетами, моделями, обучением, оценкой и публикацией ML-артефактов. |

### Установка и управление

| Репозиторий | Для чего нужен |
| --- | --- |
| [vercel-labs/skills](https://github.com/vercel-labs/skills) | Универсальный `npx skills`: установка, обновление и запуск skills в Claude Code, Codex, Cursor, Gemini CLI и десятках других агентов. |
| [numman-ali/openskills](https://github.com/numman-ali/openskills) | Универсальный загрузчик `SKILL.md`, включая агентов без нативной поддержки skills через интеграцию с `AGENTS.md`. |

### Разработка и инженерные процессы

| Репозиторий | Для чего нужен |
| --- | --- |
| [obra/superpowers](https://github.com/obra/superpowers) | Полная инженерная методология: discovery, планирование, TDD, системная отладка, code review, worktrees и multi-agent разработка. |
| [mattpocock/skills](https://github.com/mattpocock/skills) | Небольшие компонуемые skills для реальной разработки: уточнение требований, спецификации, TDD, диагностика, архитектура и ревью. |
| [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) | Официальные frontend-skills Vercel: React, Next.js, web design, деплой, производительность и оптимизация проектов. |
| [antfu/skills](https://github.com/antfu/skills) | Практики Anthony Fu и синхронизируемые skills для Vue, Nuxt, Vite, Vitest, VueUse и современного TypeScript-стека. |
| [remotion-dev/skills](https://github.com/remotion-dev/skills) | Создание программного видео с Remotion и React по рекомендациям команды Remotion. |
| [muratcankoylan/Agent-Skills-for-Context-Engineering](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering) | Context engineering, память, tool design, evaluation, multi-agent архитектуры и production agent systems. |

### Дизайн и интерфейсы

| Репозиторий | Для чего нужен |
| --- | --- |
| [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | Генерация дизайн-систем, UI/UX-рекомендации, типографика, цвета, компоненты и интерфейсы для разных платформ. |

### Исследования, знания и продуктивность

| Репозиторий | Для чего нужен |
| --- | --- |
| [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | Исследование свежей информации из Reddit, Hacker News, YouTube, X и других источников с итоговым синтезом. |
| [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) | Obsidian Markdown, Bases, JSON Canvas, CLI и работа с базой знаний. |
| [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | Более короткие и action-first ответы: следующий шаг сначала, нумерованные действия и минимум отвлечений. |

### Маркетинг и большие коллекции

| Репозиторий | Для чего нужен |
| --- | --- |
| [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | Copywriting, SEO, CRO, аналитика, customer research, email, paid ads и другие маркетинговые workflows. |
| [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) | Большая мультидоменная библиотека: engineering, product, marketing, finance, compliance, research и business operations. |

## Как устроен skill

Минимальный skill содержит только `SKILL.md`. Более сложный может включать скрипты, справочные материалы и шаблоны:

```text
my-skill/
├── SKILL.md
├── scripts/       # Необязательные исполняемые скрипты
├── references/    # Документация и дополнительные инструкции
└── assets/        # Шаблоны и статические ресурсы
```

Минимальный `SKILL.md`:

```md
---
name: angular-code-review
description: Reviews Angular code for correctness, architecture, accessibility, performance, and maintainability. Use for pull requests and code review tasks.
---

# Angular Code Review

1. Read the changed files and project conventions.
2. Find correctness and regression risks first.
3. Check Angular-specific architecture and performance.
4. Report actionable findings with file references.
5. Run or suggest the smallest relevant validation.
```

## Как создать свой skill

1. Выберите одну понятную задачу или workflow.
2. Создайте папку с `SKILL.md` и YAML frontmatter `name` + `description`.
3. В `description` явно укажите, **что делает skill и когда его активировать**.
4. Запишите конкретный процесс, проверки, ограничения и ожидаемый результат.
5. Проверьте skill на реальных запросах, включая случаи, когда он не должен активироваться.

Хороший skill не просто хранит большой prompt. Он описывает повторяемый процесс, снижает количество неоднозначных решений и дает агенту способ проверить результат.

## Как добавить проект в список

1. Создайте fork или отдельную ветку.
2. Добавьте репозиторий в подходящую категорию.
3. Напишите одно конкретное предложение: какую задачу решает проект.
4. Проверьте наличие `SKILL.md`, документации, лицензии и понятной установки.
5. Откройте Pull Request и объясните, почему проект полезен.

Подробные требования и шаблон записи находятся в [CONTRIBUTING.md](CONTRIBUTING.md).

## Безопасность

Skill может содержать команды оболочки, скрипты, сетевые запросы и инструкции по работе с секретами. Популярность репозитория не гарантирует безопасность.

Перед установкой стороннего skill:

- прочитайте `SKILL.md`, install-скрипты и содержимое `scripts/`;
- проверьте, какие файлы, команды, токены и внешние сервисы он использует;
- не передавайте секреты skill, которому они не нужны;
- для команды и CI фиксируйте проверенную версию, tag или commit;
- запускайте неизвестную автоматизацию в изолированной среде.

## Contributing

Pull Requests приветствуются. См. [CONTRIBUTING.md](CONTRIBUTING.md).
