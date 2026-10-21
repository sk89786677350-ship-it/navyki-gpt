# Навыки GPT

Проверенный реестр глобальных навыков Codex по состоянию на 21 октября 2026 года. В папке навыков обнаружены **47 уникальных папок с `SKILL.md`**: 34 навыка из предыдущей сверки, расширенный и переименованный личный навык `website-research-brief`, а также личные навыки `website-niche-research`, `elite-marketer`, `personal-tutor`, `project-continuity` и `personal-planner`, `verified-completion` и `project-repository-sync` и `skillsmp-agent`. В прежней версии этого реестра было 14 названий; затем добавлены 20 недостающих. Системные навыки Codex в число 47 не входят.

Репозиторий содержит перечень и ссылки на первоисточники. Он сам по себе не устанавливает навыки на другой компьютер. Исходные файлы сторонних навыков, личные пути, ключи доступа и данные проектов сюда не копируются. Содержимое созданных пользователем личных навыков может публиковаться с его разрешения.

## Все глобальные навыки

Каждое название в таблице указано один раз.

| Направление | Навыки | Число | Для чего |
| --- | --- | ---: | --- |
| Интервью | `discovery-interview-prep`, `ux-discovery-interviewer`, `discovery-interview` | 3 | Подготовка и проведение интервью |
| Исследование продукта | `jobs-to-be-done`, `problem-statement`, `proto-persona`, `workshop-facilitation` | 4 | Потребности клиентов, формулировка проблемы, персона и фасилитация |
| Дизайн | `ui-ux-pro-max`, `frontend-design`, `design-taste-frontend` | 3 | Интерфейсы и визуальное оформление |
| Сайт, данные и выпуск | `fullstack-engineer`, `database-engineer`, `data-engineer`, `qa-engineer`, `security-engineer`, `devops`, `website-niche-research`, `website-research-brief` | 8 | Разработка, данные, качество, безопасность, развёртывание, исследование ниши и подготовка ТЗ для сайта или веб-продукта |
| Маркетинг и рост бизнеса | `elite-marketer` | 1 | Позиционирование, аудитория, оффер и возможности роста |
| Обучение и учебные продукты | `personal-tutor` | 1 | Индивидуальные программы по предметам, ПО и навыкам; учебные проекты и продукты |
| Проектная работа | `project-continuity` | 1 | Фактические контрольные точки и перенос контекста между Codex и ChatGPT |
| Синхронизация проектов | `project-repository-sync` | 1 | Сверка локальной папки с соответствующим удалённым репозиторием |
| Личное планирование | `personal-planner` | 1 | Разбор личных дел и реалистичное планирование в Codex и ChatGPT |
| Проверка готовности | `verified-completion` | 1 | Критерии приёмки, проверка результата и честная сводка о выполненном и оставшемся |
| Клиентские AI-агенты | `ai-engineer`, `prompt-engineer`, `llm-tester` | 3 | Архитектура, инструкции и оценка ответов |
| Видео | `remotion-best-practices` | 1 | Анимация и монтаж на Remotion |
| Движение и анимация | `animate`, `review-animations`, `improve-animations` | 3 | Создание, обзор и аудит движения в интерфейсах |
| Методы разработки Superpowers | `brainstorming`, `diagnosing-superpowers`, `dispatching-parallel-agents`, `executing-plans`, `finishing-a-development-branch`, `receiving-code-review`, `requesting-code-review`, `subagent-driven-development`, `systematic-debugging`, `test-driven-development`, `using-git-worktrees`, `using-superpowers`, `verification-before-completion`, `writing-plans`, `writing-skills` | 15 | Планирование, исполнение, отладка, проверки и завершение работы |
| Поиск навыков | `skillsmp-agent` | 1 | Поиск, сравнение и проверка навыков SkillsMP перед установкой |
| **Итого** | **47 уникальных навыков** | **47** | |

Пятнадцать навыков Superpowers есть в глобальной папке и в установленном плагине. Файлы `SKILL.md` в этих двух местах совпали по SHA-256; это **одни и те же навыки**, они посчитаны один раз. Отдельно доступны системный `imagegen` и инструменты Higgsfield; они не входят в число 42 глобальных папок.

## Первоисточники и версии

- **Личные навыки:** [skillsmp-agent](skills/skillsmp-agent/SKILL.md) добавлен для безопасного поиска и проверки сообщества SkillsMP; его workflow основан на [официальной документации SkillsMP API](https://skillsmp.com/docs/api) и [документации OpenAI по навыкам](https://learn.chatgpt.com/docs/build-skills). [website-niche-research](skills/website-niche-research/SKILL.md) исследует нишу любого нового сайта или веб-продукта; [website-research-brief](skills/website-research-brief/SKILL.md) готовит полное проектное ТЗ для сайтов и веб-продуктов; [elite-marketer](skills/elite-marketer/SKILL.md) помогает с позиционированием, аудиторией, оффером и ростом; [project-continuity](skills/project-continuity/SKILL.md) сохраняет контрольные точки и готовит перенос контекста между Codex и ChatGPT; [полный промпт project-continuity](skills/project-continuity/references/project-continuity-prompt.md); [personal-planner](skills/personal-planner/SKILL.md) помогает с личными задачами и планом дня или недели; комплект содержит [полный промпт ChatGPT](skills/personal-planner/references/personal-chatgpt-planner-prompt.md), [инструкции ChatGPT и Codex](skills/personal-planner/references/) и [шаблон файлов личной папки](skills/personal-planner/references/personal-planner-folder-template/); [verified-completion](skills/verified-completion/SKILL.md) помогает сверять существенные задачи с проверяемыми критериями; доступны [полный промпт](skills/verified-completion/references/verified-completion-prompt.md) и [инструкция запуска](skills/verified-completion/references/verified-completion-start.md). [personal-tutor](skills/personal-tutor/SKILL.md) создает индивидуальные программы обучения, сопровождает учебные проекты и помогает проектировать учебные продукты. Опубликованы [полный промпт](skills/personal-tutor/references/personal-tutor-prompt.md) и [подробная методика](skills/personal-tutor/references/personal-tutor-learning-system.md) с разрешения владельца. [project-repository-sync](skills/project-repository-sync/SKILL.md) сверяет изменения локального проекта с соответствующим репозиторием и готовит продолжение работы.
- **Superpowers, 15 навыков:** [obra/superpowers](https://github.com/obra/superpowers), установленный плагин версии `6.4.2`, лицензия MIT. Локальные копии основных файлов сверены с плагином.
- **Исследование продукта, 5 навыков** (включая `discovery-interview-prep`): [deanpeters/Product-Manager-Skills](https://github.com/deanpeters/Product-Manager-Skills). Совпадение названий и расположения у автора подтверждено; точная версия локальных файлов не установлена. [Условия CC BY-NC-SA 4.0](https://github.com/deanpeters/Product-Manager-Skills#license) разрешают использование в работе, но ограничивают продажу и перепаковку самих навыков.
- **Дизайн:** `ui-ux-pro-max` — [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill), коммит `56ea9cf174ed86786187daa9de0e6247cb0747e4`; `frontend-design` — [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/frontend-design), коммит `dbd4588f9e1033efb41dad4bef2f7947c8993d44`; `design-taste-frontend` — [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill), версия `2.0.0`, коммит `f624f37a8c650b9cc550253104925efe4c8de246`, MIT.
- **Движение и анимация:** `animate`, `review-animations`, `improve-animations` — [emilkowalski/skills](https://github.com/emilkowalski/skills), коммит `2d228630ba1446365f614a108cb8252f1feda202`, MIT. `review-animations` запускается только по явному запросу.
- Правила выбора этих навыков для сайтов собраны в [маршрутизации дизайн-навыков](skills/website-research-brief/references/design-skill-routing.md).
- **Сайт, данные и AI-агенты, 9 навыков:** [buiphucminhtam/forgewright](https://github.com/buiphucminhtam/forgewright/tree/main/skills), коммит `1b652cee8fb51fa4241049c4d37ae0f5826a8025`. Общая лицензия репозитория не подтверждена.
- **Видео:** `remotion-best-practices` — [remotion-dev/skills](https://github.com/remotion-dev/skills/tree/main/skills/remotion-best-practices), коммит `1441a11e95db35443bd76bb318386c0d3ca00053`.
- **Источник требует уточнения:** `discovery-interview` и `ux-discovery-interviewer`. Они реально установлены локально, но автор и точная исходная версия не подтверждены. Публичные проекты с похожими названиями не считаются доказательством происхождения этих файлов.

## Ограничения восстановления

- Глобальные навыки на Lenovo доступны Codex локально. Этот список служит учётом, а не полной резервной копией файлов.
- Отдельные навыки Forgewright ссылаются на общие правила полного набора; полная среда не устанавливалась.
- У `ui-ux-pro-max` локально адаптирован путь к поисковому скрипту; на другом компьютере его нужно настроить заново.
- Установка не подключала платные API, видеосервисы или движок Remotion. [Условия Remotion](https://www.remotion.dev/docs/license/pricing) проверяются под конкретный проект.
- Для задач по заказам и остаткам нужна актуальная таблица склада и точное сопоставление артикулов.
