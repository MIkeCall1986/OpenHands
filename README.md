<a name="readme-top"></a>

<div align="center">
  <img src="https://raw.githubusercontent.com/OpenHands/docs/main/openhands/static/img/logo.png" alt="Logo" width="200">
  <h1 align="center" style="border-bottom: none">OpenHands: AI-Driven Development</h1>
</div>


<div align="center">
  <a href="https://github.com/OpenHands/OpenHands/blob/main/LICENSE"><img src="https://img.shields.io/badge/LICENSE-MIT-20B2AA?style=for-the-badge" alt="MIT License"></a>
  <a href="https://docs.google.com/spreadsheets/d/1wOUdFCMyY6Nt0AIqF705KN4JKOWgeI4wUGUP60krXXs/edit?gid=811504672#gid=811504672"><img src="https://img.shields.io/badge/SWEBench-77.6-00cc00?logoColor=FFE165&style=for-the-badge" alt="Benchmark Score"></a>
  <br/>
  <a href="https://docs.openhands.dev/sdk"><img src="https://img.shields.io/badge/Documentation-000?logo=googledocs&logoColor=FFE165&style=for-the-badge" alt="Check out the documentation"></a>
  <a href="https://arxiv.org/abs/2511.03690"><img src="https://img.shields.io/badge/Paper-000?logoColor=FFE165&logo=arxiv&style=for-the-badge" alt="Tech Report"></a>


  <!-- Keep these links. Translations will automatically update with the README. -->
  <a href="https://www.readme-i18n.com/OpenHands/OpenHands?lang=de">Deutsch</a> |
  <a href="https://www.readme-i18n.com/OpenHands/OpenHands?lang=es">Español</a> |
  <a href="https://www.readme-i18n.com/OpenHands/OpenHands?lang=fr">français</a> |
  <a href="https://www.readme-i18n.com/OpenHands/OpenHands?lang=ja">日本語</a> |
  <a href="https://www.readme-i18n.com/OpenHands/OpenHands?lang=ko">한국어</a> |
  <a href="https://www.readme-i18n.com/OpenHands/OpenHands?lang=pt">Português</a> |
  <a href="https://www.readme-i18n.com/OpenHands/OpenHands?lang=ru">Русский</a> |
  <a href="https://www.readme-i18n.com/OpenHands/OpenHands?lang=zh">中文</a>

</div>

<hr>

🙌 Welcome to OpenHands, a [community](COMMUNITY.md) focused on AI-driven development. We’d love for you to [join us on Slack](https://dub.sh/openhands).

There are a few ways to work with OpenHands:

### OpenHands Software Agent SDK
The SDK is a composable Python library that contains all of our agentic tech. It's the engine that powers everything else below.

Define agents in code, then run them locally, or scale to 1000s of agents in the cloud.

[Check out the docs](https://docs.openhands.dev/sdk) or [view the source](https://github.com/OpenHands/software-agent-sdk/)

### OpenHands CLI
The CLI is the easiest way to start using OpenHands. The experience will be familiar to anyone who has worked
with e.g. Claude Code or Codex. You can power it with Claude, GPT, or any other LLM.

[Check out the docs](https://docs.openhands.dev/openhands/usage/run-openhands/cli-mode) or [view the source](https://github.com/OpenHands/OpenHands-CLI)

### OpenHands Local GUI
Use the Local GUI for running agents on your laptop. It comes with a REST API and a single-page React application.
The experience will be familiar to anyone who has used Devin or Jules.

[Check out the docs](https://docs.openhands.dev/openhands/usage/run-openhands/local-setup) or view the source in this repo.

### OpenHands Cloud
This is a deployment of OpenHands GUI, running on hosted infrastructure.

You can try it for free using the Minimax model by [signing in with your GitHub or GitLab account](https://app.all-hands.dev).

OpenHands Cloud comes with source-available features and integrations:
- Integrations with Slack, Jira, and Linear
- Multi-user support
- RBAC and permissions
- Collaboration features (e.g., conversation sharing)

### OpenHands Enterprise
Large enterprises can work with us to self-host OpenHands Cloud in their own VPC, via Kubernetes.
OpenHands Enterprise can also work with the CLI and SDK above.

OpenHands Enterprise is source-available--you can see all the source code here in the enterprise/ directory,
but you'll need to purchase a license if you want to run it for more than one month.

Enterprise contracts also come with extended support and access to our research team.

Learn more at [openhands.dev/enterprise](https://openhands.dev/enterprise)

### Everything Else

Check out our [Product Roadmap](https://github.com/orgs/openhands/projects/1), and feel free to
[open up an issue](https://github.com/OpenHands/OpenHands/issues) if there's something you'd like to see!

You might also be interested in our [evaluation infrastructure](https://github.com/OpenHands/benchmarks), our [chrome extension](https://github.com/OpenHands/openhands-chrome-extension/), or our [Theory-of-Mind module](https://github.com/OpenHands/ToM-SWE).

All our work is available under the MIT license, except for the `enterprise/` directory in this repository (see the [enterprise license](enterprise/LICENSE) for details).
The core `openhands` and `agent-server` Docker images are fully MIT-licensed as well.

If you need help with anything, or just want to chat, [come find us on Slack](https://dub.sh/openhands).

20.02.26 sync fork 
Ось результати аналізу та стратегія трансформації для проекту **OpenHands**, підготовлені у форматі для копіювання в Notion.

---

# 📑 Звіт AI-консультанта: Проект "OpenHands"

**OpenHands** — це платформа та спільнота, орієнтована на розробку за допомогою ШІ-агентів під гаслом "Пиши менше, створюй більше".

---

## 🧬 Частина 1: "ДНК" Проекту

Логіку коду проекту можна розбити на такі **атомарні функції**:

*   **Оркестрація агентів (Agentic Engine):** Використання SDK як компонованої бібліотеки Python для визначення, запуску та масштабування ШІ-агентів локально або в хмарі.
*   **Інтерфейсна взаємодія (CLI & GUI):** Надання доступу до функцій через командний рядок (аналогічно Claude Code) або через веб-інтерфейс (React-застосунок) з використанням REST API.
*   **Інтеграція зовнішніх інструментів:** Підключення до Slack, Jira та Linear для забезпечення спільної роботи та управління задачами.
*   **Управління доступом (RBAC & Auth):** Система багатокористувацької підтримки, дозволів та безпечного розгортання в корпоративних мережах через Kubernetes.
*   **Цикл розробки (CI/CD):** Автоматизація робочих процесів через GitHub Actions та підтримка середовищ розробки.

### 💎 Головна технічна цінність
Головна цінність OpenHands полягає в створенні **універсального рушія для ШІ-агентів (Agent SDK)**, який дозволяє перетворити статичний код на автономну систему, що здатна самостійно писати, виправляти та масштабувати програмне забезпечення. Це міст між потужністю мовних моделей та практичним виконанням коду.

---

## 🚀 Частина 2: "Трансформація" (Інтеграція з Gemini LLM)

Додавання мультимодальних можливостей **Gemini** (через **GitHub Models**) перетворює OpenHands на **автономну "фабрику" застосунків**.

### Як зміниться функціонал?
1.  **Мультимодальне бачення коду:** Gemini зможе аналізувати не лише текст коду, а й макети дизайну або скріншоти помилок, автоматично виправляючи фронтенд-частину через OpenHands GUI.
2.  **Глибоке контекстне вікно:** Завдяки великому контексту Gemini, агенти OpenHands зможуть розуміти архітектуру всього репозиторію одночасно, а не окремих файлів, що значно підвищує якість рефакторингу.
3.  **Інтелектуальне планування:** ШІ зможе самостійно розбивати великі бізнес-задачі на технічні тікети в Jira/Linear і виконувати їх без втручання людини.

### Сценарій сервісу "AI-App-Factory" (OpenHands + Gemini + ID_{$})

Сценарій створення сервісу автоматичного створення мікросервісів на вашому сайті:
1.  **Запит клієнта:** Користувач на вашому сайті описує ідею: *"Створи сервіс для аналізу акцій"*.
2.  **Підготовка даних (ID_{$}):** Ваші базові Python-скрипти **ID_{$}** збирають актуальну інформацію з фінансових ринків.
3.  **Розробка (OpenHands + Gemini):** OpenHands отримує дані від скриптів і за допомогою **Gemini** генерує повний код бекенду та фронтенду, базуючись на кращих практиках.
4.  **Валідація та тести:** Агенти OpenHands самостійно запускають тести та виправляють баги в ізольованому середовищі.
5.  **Розгортання (GitHub Spark):** Готовий код автоматично деплоїться через **GitHub Spark** як робочий інтелектуальний застосунок.

---

## 📋 План дій для Notion
| Крок | Дія | Результат |
| :--- | :--- | :--- |
| **1** | Встановлення **OpenHands SDK** (`pip install openhands-sdk`) | Ядро ШІ-агента у вашому проекті |
| **2** | Підключення Gemini через **GitHub Models** | "Мізки" для прийняття архітектурних рішень |
| **3** | Інтеграція ваших скриптів `ID_{$}` як "інструментів" (tools) для агента | Автоматизація збору специфічних даних |
| **4** | Використання **GitHub Spark** для швидкого деплою фронтенду | Готовий сервіс на вашому домені |

---

### 💡 Резюме

**Суть:** **Платформа для розробки через ШІ-агентів**.

**AI-Роль:** **Побудова інтелектуальних застосунків через Spark**.
