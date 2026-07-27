<div align="center">

# Awesome AI Skills

**Курируемая коллекция Agent Skills для Claude Code, Codex, Gemini CLI, GitHub Copilot, Cursor и других AI-агентов.**

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

</div>

Каталог практических skills для разработки, тестирования, дизайна, исследований и других задач.

> Новичкам: [что такое Agent Skills, как их устанавливать и создавать](docs/guide.md).
>
> **Последняя проверка списка:** 27 июля 2026 года. Популярность учитывается, но не является единственным критерием: также важны практическая польза, документация, лицензия и активность проекта.

## Каталог

- [Стандарт и официальные коллекции](#стандарт-и-официальные-коллекции)
- [Установка и управление](#установка-и-управление)
- [Разработка и инженерные процессы](#разработка-и-инженерные-процессы)
- [JavaScript и тестирование](#javascript-и-тестирование)
- [Дизайн и интерфейсы](#дизайн-и-интерфейсы)
- [Исследования, знания и продуктивность](#исследования-знания-и-продуктивность)
- [Маркетинг и большие коллекции](#маркетинг-и-большие-коллекции)

### Стандарт и официальные коллекции

| Репозиторий | Для чего нужен |
| --- | --- |
| [agentskills/agentskills](https://github.com/agentskills/agentskills) | Открытая спецификация Agent Skills, документация и правила совместимости. |
| [anthropics/skills](https://github.com/anthropics/skills) | Официальные примеры Anthropic: документы, таблицы, PDF, презентации, дизайн и технические workflows. |
| [openai/plugins](https://github.com/openai/plugins) | Актуальная коллекция плагинов Codex со skills, MCP, agents, commands и другими расширениями. |
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
| [openai/plugins: security-scan](https://github.com/openai/plugins/tree/main/plugins/codex-security/skills/security-scan) | Проводит последовательный security-аудит репозитория или выбранной директории: строит threat model, ищет и проверяет уязвимости, анализирует attack paths и формирует отчет. |
| [openai/plugins: gh-fix-ci](https://github.com/openai/plugins/tree/main/plugins/github/skills/gh-fix-ci) | Диагностирует падающие проверки GitHub Actions в Pull Request через GitHub-контекст и `gh`, объясняет причину и готовит план исправления перед внесением изменений. |
| [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) | Официальные frontend-skills Vercel: React, Next.js, web design, деплой, производительность и оптимизация проектов. |
| [antfu/skills](https://github.com/antfu/skills) | Практики Anthony Fu и синхронизируемые skills для Vue, Nuxt, Vite, Vitest, VueUse и современного TypeScript-стека. |
| [remotion-dev/skills](https://github.com/remotion-dev/skills) | Создание программного видео с Remotion и React по рекомендациям команды Remotion. |
| [muratcankoylan/Agent-Skills-for-Context-Engineering](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering) | Context engineering, память, tool design, evaluation, multi-agent архитектуры и production agent systems. |

### JavaScript и тестирование

| Skill | Для чего нужен |
| --- | --- |
| [LambdaTest/agent-skills: karma-skill](https://github.com/LambdaTest/agent-skills/tree/main/karma-skill) | Настраивает Karma для браузерных JavaScript/TypeScript-тестов: frameworks, browsers, coverage, reporters и запуск в CI. |
| [LambdaTest/agent-skills: jasmine-skill](https://github.com/LambdaTest/agent-skills/tree/main/jasmine-skill) | Помогает писать Jasmine-тесты со spies, matchers и асинхронными сценариями. Хорошее дополнение к Karma-проектам. |
| [obra/superpowers: systematic-debugging](https://github.com/obra/superpowers/tree/main/skills/systematic-debugging) | Ведет от воспроизведения ошибки и сбора фактов к поиску первопричины, проверке гипотез и минимальному исправлению. |
| [obra/superpowers: verification-before-completion](https://github.com/obra/superpowers/tree/main/skills/verification-before-completion) | Требует запускать актуальные проверки и читать их результат перед утверждением, что задача завершена или исправление работает. |
| [obra/superpowers: requesting-code-review](https://github.com/obra/superpowers/tree/main/skills/requesting-code-review) | Формирует контекст для отдельного code-review перед завершением крупной задачи или merge. |
| [obra/superpowers: test-driven-development](https://github.com/obra/superpowers/tree/main/skills/test-driven-development) | Задает строгий цикл RED–GREEN–REFACTOR: сначала падающий тест, затем минимальная реализация и рефакторинг. |
| [LambdaTest/agent-skills: cicd-pipeline-skill](https://github.com/LambdaTest/agent-skills/tree/main/cicd-pipeline-skill) | Генерирует CI/CD-конфигурации для автоматизированных тестов в GitHub Actions, GitLab CI, Jenkins и Azure DevOps. |

Для проекта на Karma и Jasmine базовый набор: `karma-skill`, `jasmine-skill`, `systematic-debugging` и `verification-before-completion`. TDD, code review и CI/CD skills можно подключать по процессам команды.

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

## Участие

Pull Requests приветствуются. Требования и формат записи находятся в [CONTRIBUTING.md](CONTRIBUTING.md).

Перед установкой сторонних skills прочитайте раздел [Безопасность](docs/guide.md#безопасность).
