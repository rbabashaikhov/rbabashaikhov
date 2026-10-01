<table border=0>
  <tr>
    <td width="180" valign="top">
      <img src="https://avatars.githubusercontent.com/u/83781078?v=4" width="150" />
    </td>
    <td valign="top">
      <h1>Привет, я Руслан Бабашаихов 👋</h1>
      <h3>AI • Automation • Data Engineer</h3>
      <p>
        Разрабатываю практические AI-системы и автоматизации — от прототипов и RAG-пайплайнов до работающих приложений, развернутых в production.
      </p>
      <p>
        Мой бэкграунд — веб- и продуктовая аналитика. Сейчас основной фокус — <b>LLM-приложения, RAG, AI-агенты, автоматизация бизнес-процессов и Python-разработка</b>.
      </p>
    </td>
  </tr>
</table>

---

<p align="center">
  <img height="150em" src="https://github-readme-stats.vercel.app/api?username=rbabashaikhov&show_icons=true&theme=algolia&hide_border=true" />
  <img height="150em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=rbabashaikhov&layout=compact&theme=algolia&hide_border=true" />
</p>

---

## 🛠 Технологии

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

`LLM` · `RAG` · `AI Agents` · `Prompt Engineering` · `pgvector` · `REST API` · `Telegram Bots` · `Docker Compose` · `VPS` · `SQL` · `Analytics`

---

## 🚀 Что я разрабатываю

- 🤖 **LLM-приложения** — RAG-системы, AI-ассистенты и специализированные агенты
- 🔎 **Retrieval-системы** — embeddings, векторный поиск, reranking и оценка качества поиска
- ⚙️ **AI-автоматизации** — n8n, API-интеграции и автоматизация бизнес-процессов
- 🐳 **Production-инфраструктуру** — Docker, Linux, VPS, PostgreSQL, reverse proxy и мониторинг
- 📊 **Data & Analytics** — SQL, Power BI, пайплайны данных, продуктовая и веб-аналитика
- 📱 **Прикладные продукты** — Telegram-боты, Mini Apps и веб-приложения

---

# 🔥 Ключевые проекты

## 🧠 Enterprise Private GPT

**Полностью локальный RAG-ассистент для работы с юридическими документами.**

Документы, embeddings, векторная база и LLM работают внутри собственной инфраструктуры без внешних LLM API.

**Архитектура**

`Документы → Chunking → Embeddings → Qdrant → Retrieval → Relevance Gate → Local LLM → Ответ`

**Стек:**  
`Python` · `LangChain` · `Qdrant` · `multilingual-e5-small` · `Ollama` · `Qwen2.5` · `Streamlit` · `Docker`

Что реализовано:

- локальный inference через Ollama
- семантический поиск в Qdrant
- relevance threshold для отсечения нерелевантных запросов
- измерение retrieval / generation latency
- эксперименты с Top-K
- evaluation retrieval-качества
- приватный доступ через SSH tunnel

👉 [Репозиторий](https://github.com/rbabashaikhov/enterprise-private-gpt)

---

## 📺 Samsung TV AI Consultant

**AI-консультант по каталогу телевизоров Samsung с production-oriented архитектурой.**

Проект сочетает структурированные данные о товарах с LLM reasoning и retrieval, а не полагается только на векторное сходство.

**Стек:**  
`Python` · `PostgreSQL` · `pgvector` · `OpenAI` · `n8n` · `Docker`

В проекте реализованы и исследованы:

- структурированный каталог товаров
- vector и structured retrieval
- RAG
- agent tools
- intent semantics
- retrieval evaluation
- сравнение моделей
- защита от hallucinations и фактических ошибок
- multi-turn dialogue
- автоматизированные evaluation suites

Проект развивается внутри моего AI Automation Lab.

👉 [AI Automation Lab](https://github.com/rbabashaikhov/ai-automation-lab)

---

## 🔐 n8n Workflow-as-Code Tool

CLI-инструмент для управления n8n workflow через официальный REST API.

Основная идея — сделать разработку и обновление автоматизаций более управляемыми и Git-friendly.

Реализовано:

- discovery и export workflow
- безопасное обновление workflow
- diff перед применением изменений
- подтверждение перед write-операциями
- проверка на секреты
- reusable tooling для автоматизаций

👉 [AI Automation Lab](https://github.com/rbabashaikhov/ai-automation-lab)

---

## ⚖️ Legal NER с YandexGPT

Эксперимент по извлечению именованных сущностей из юридических документов с помощью LLM.

Проект посвящен structured entity extraction из русскоязычных юридических текстов.

**Стек:**  
`Python` · `YandexGPT` · `Yandex AI SDK` · `uv`

👉 [Репозиторий](https://github.com/rbabashaikhov/OTUS-08-YandexGPT)

---

## 🥗 AI Food Coach

Production Telegram-бот, который анализирует еду по фотографии и дает персонализированную обратную связь.

Функции:

- анализ блюда по фото
- follow-up вопросы
- рекомендации по питанию
- анализ рациона за день
- подписки
- онлайн-оплата
- хранение данных в PostgreSQL
- production deployment

**Стек:**  
`Python` · `aiogram` · `OpenAI Vision` · `PostgreSQL` · `Docker` · `YooKassa`

🤖 [Открыть AI Food Coach](https://t.me/ai_food_coach_bot)

---

## 🎮 Two Goblins

Экспериментальная браузерная кооперативная игра для двух игроков через интернет.

**Стек:**  
`Phaser` · `Colyseus` · `Node.js` · `WebSocket` · `Docker` · `Caddy`

Реализовано:

- multiplayer rooms
- real-time синхронизация
- invite links
- reconnect
- мобильное управление
- переход между уровнями
- система очков
- telemetry сетевой задержки

🎮 [Играть](https://goblins.leadmeter.ru)

---

## 📊 SEO Analytics Pipeline

Проект по сбору, трансформации и анализу SEO-данных.

Он отражает мой аналитический бэкграунд и сочетает data engineering с прикладной аналитикой.

👉 [Репозиторий](https://github.com/rbabashaikhov/seo-analytics-pipeline)

---

## 🧪 Другие проекты

### AI CRM Email Builder

AI-инструменты и автоматизация для работы с CRM-коммуникациями.

👉 [Репозиторий](https://github.com/rbabashaikhov/ai-crm-email-builder)

### Telegram Mini Apps и веб-приложения

Разрабатываю Telegram Mini Apps и прикладные веб-сервисы для бизнеса: запись на услуги, beauty, automotive, real estate и другие направления.

🌐 [Портфолио проектов](https://apps.leadmeter.ru)

---

# 🧩 На чем сейчас фокусируюсь

- **RAG quality & evaluation**
- **AI agents и tool use**
- **hybrid / structured retrieval**
- **LLM guardrails**
- **workflow automation**
- **local / private LLM**
- **production AI observability**
- **AI-приложения для бизнеса**

---

## 💡 Подход к разработке

Мне интересны не просто эффектные AI-демо, а системы, которые можно **измерять, тестировать, поддерживать и разворачивать в production**.

Для AI-проектов я смотрю на весь цикл:

`Retrieval quality → Grounding → Evaluation → Latency → Cost → Reliability → Production`

---

## 🌐 Ссылки

[![Portfolio](https://img.shields.io/badge/Portfolio-leadmeter.ru-0A66C2?style=for-the-badge)](https://apps.leadmeter.ru)
[![GitHub](https://img.shields.io/badge/GitHub-rbabashaikhov-181717?style=for-the-badge&logo=github)](https://github.com/rbabashaikhov)

---

### Открыт к проектам и предложениям в направлениях

**AI Engineering · AI Automation · LLM / RAG · Data & Analytics**
