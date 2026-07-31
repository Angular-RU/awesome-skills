<div align="center">

# Awesome AI Skills

**Курируемая коллекция Agent Skills для Claude Code, Codex, Gemini CLI, GitHub Copilot, Cursor и других AI-агентов.**

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

</div>

Каталог практических skills для разработки, тестирования, дизайна, исследований и других задач.

> Новичкам: [что такое Agent Skills, как их устанавливать и создавать](docs/guide.md).
>
> **Последняя проверка списка:** 31 июля 2026 года. Популярность учитывается, но не является единственным критерием: также важны практическая польза, документация, лицензия и активность проекта.

## Каталог

* [Стандарт и официальные коллекции](#стандарт-и-официальные-коллекции)
* [Установка и управление](#установка-и-управление)
* [Разработка и инженерные процессы](#разработка-и-инженерные-процессы)
* [JavaScript и тестирование](#javascript-и-тестирование)
* [Дизайн и интерфейсы](#дизайн-и-интерфейсы)
* [Исследования, знания и продуктивность](#исследования-знания-и-продуктивность)
* [Маркетинг и большие коллекции](#маркетинг-и-большие-коллекции)

### Стандарт и официальные коллекции

* [agentskills/agentskills](https://github.com/agentskills/agentskills) - открытая спецификация Agent Skills, документация и правила совместимости.
* [anthropics/skills](https://github.com/anthropics/skills) - официальные примеры Anthropic: документы, таблицы, PDF, презентации, дизайн и технические workflows.
* [openai/plugins](https://github.com/openai/plugins) - актуальная коллекция плагинов Codex со skills, MCP, agents, commands и другими расширениями.
* [google/skills](https://github.com/google/skills) - официальные skills для Google Cloud, Gemini API, Firebase, BigQuery, Cloud Run, GKE и архитектурных практик.
* [microsoft/skills](https://github.com/microsoft/skills) - skills, custom agents и MCP-конфигурации для Azure SDK, Microsoft Foundry и облачной разработки.
* [huggingface/skills](https://github.com/huggingface/skills) - работа с Hugging Face Hub, датасетами, моделями, обучением, оценкой и публикацией ML-артефактов.

### Установка и управление

* [vercel-labs/skills](https://github.com/vercel-labs/skills) - универсальный `npx skills`: установка, обновление и запуск skills в Claude Code, Codex, Cursor, Gemini CLI и десятках других агентов.
* [numman-ali/openskills](https://github.com/numman-ali/openskills) - универсальный загрузчик `SKILL.md`, включая агентов без нативной поддержки skills через интеграцию с `AGENTS.md`.

### Разработка и инженерные процессы

* [obra/superpowers](https://github.com/obra/superpowers) - полная инженерная методология: discovery, планирование, TDD, системная отладка, code review, worktrees и multi-agent разработка.
* [mattpocock/skills](https://github.com/mattpocock/skills) - небольшие компонуемые skills для реальной разработки: уточнение требований, спецификации, TDD, диагностика, архитектура и ревью.
* [openai/plugins: security-scan](https://github.com/openai/plugins/tree/main/plugins/codex-security/skills/security-scan) - проводит последовательный security-аудит репозитория или выбранной директории: строит threat model, ищет и проверяет уязвимости, анализирует attack paths и формирует отчет.
* [zhaoxuya520/reverse-skill](https://github.com/zhaoxuya520/reverse-skill) - маршрутизирует авторизованные задачи reverse engineering и security-анализа по специализированным skills для APK, бинарных файлов, JavaScript, malware, firmware и CTF с обязательной фиксацией scope и доказательств.
* [openai/plugins: gh-fix-ci](https://github.com/openai/plugins/tree/main/plugins/github/skills/gh-fix-ci) - диагностирует падающие проверки GitHub Actions в Pull Request через GitHub-контекст и `gh`, объясняет причину и готовит план исправления перед внесением изменений.
* [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) - официальные frontend-skills Vercel: React, Next.js, web design, деплой, производительность и оптимизация проектов.
* [antfu/skills](https://github.com/antfu/skills) - практики Anthony Fu и синхронизируемые skills для Vue, Nuxt, Vite, Vitest, VueUse и современного TypeScript-стека.
* [remotion-dev/skills](https://github.com/remotion-dev/skills) - создание программного видео с Remotion и React по рекомендациям команды Remotion.
* [muratcankoylan/Agent-Skills-for-Context-Engineering](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering) - context engineering, память, tool design, evaluation, multi-agent архитектуры и production agent systems.

### JavaScript и тестирование

* [LambdaTest/agent-skills: karma-skill](https://github.com/LambdaTest/agent-skills/tree/main/karma-skill) - настраивает Karma для браузерных JavaScript/TypeScript-тестов: frameworks, browsers, coverage, reporters и запуск в CI.
* [LambdaTest/agent-skills: jasmine-skill](https://github.com/LambdaTest/agent-skills/tree/main/jasmine-skill) - помогает писать Jasmine-тесты со spies, matchers и асинхронными сценариями. Хорошее дополнение к Karma-проектам.
* [obra/superpowers: systematic-debugging](https://github.com/obra/superpowers/tree/main/skills/systematic-debugging) - ведет от воспроизведения ошибки и сбора фактов к поиску первопричины, проверке гипотез и минимальному исправлению.
* [obra/superpowers: verification-before-completion](https://github.com/obra/superpowers/tree/main/skills/verification-before-completion) - требует запускать актуальные проверки и читать их результат перед утверждением, что задача завершена или исправление работает.
* [obra/superpowers: requesting-code-review](https://github.com/obra/superpowers/tree/main/skills/requesting-code-review) - формирует контекст для отдельного code-review перед завершением крупной задачи или merge.
* [obra/superpowers: test-driven-development](https://github.com/obra/superpowers/tree/main/skills/test-driven-development) - задает строгий цикл RED-GREEN-REFACTOR: сначала падающий тест, затем минимальная реализация и рефакторинг.
* [LambdaTest/agent-skills: cicd-pipeline-skill](https://github.com/LambdaTest/agent-skills/tree/main/cicd-pipeline-skill) - генерирует CI/CD-конфигурации для автоматизированных тестов в GitHub Actions, GitLab CI, Jenkins и Azure DevOps.

Для проекта на Karma и Jasmine базовый набор: `karma-skill`, `jasmine-skill`, `systematic-debugging` и `verification-before-completion`. TDD, code review и CI/CD skills можно подключать по процессам команды.

### Дизайн и интерфейсы

* [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) - генерация дизайн-систем, UI/UX-рекомендации, типографика, цвета, компоненты и интерфейсы для разных платформ.

### Исследования, знания и продуктивность

* [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) - исследование свежей информации из Reddit, Hacker News, YouTube, X и других источников с итоговым синтезом.
* [virgiliojr94/book-to-skill](https://github.com/virgiliojr94/book-to-skill) - превращает книги и наборы документов PDF, EPUB, DOCX, Markdown и других форматов в структурированные Agent Skills с главами, глоссарием, паттернами и шпаргалкой для загрузки знаний по запросу.
* [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) - Obsidian Markdown, Bases, JSON Canvas, CLI и работа с базой знаний.
* [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) - более короткие и action-first ответы: следующий шаг сначала, нумерованные действия и минимум отвлечений.

### Маркетинг и большие коллекции

* [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) - copywriting, SEO, CRO, аналитика, customer research, email, paid ads и другие маркетинговые workflows.
* [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) - большая мультидоменная библиотека: engineering, product, marketing, finance, compliance, research и business operations.

## Участие

Pull Requests приветствуются. Требования и формат записи находятся в [CONTRIBUTING.md](CONTRIBUTING.md).

Перед установкой сторонних skills прочитайте раздел [Безопасность](docs/guide.md#безопасность).
