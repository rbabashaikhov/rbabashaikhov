# 👋 Привет, я Руслан Бабашаихов

### AI Engineering · Automation · Data

Разрабатываю прикладные AI- и data-системы для бизнеса: **RAG/LLM-приложения, AI-ассистенты, автоматизацию процессов, интеграции, ETL/аналитические пайплайны и BI**.

Мой бэкграунд — веб- и продуктовая аналитика. Поэтому в проектах я смотрю не только на код, но и на качество данных, измеримость результата, стоимость эксплуатации и надёжность решения.

**Открыт к проектам и сотрудничеству.**

[🌐 Портфолио](https://apps.leadmeter.ru) · [💼 Leadmeter](https://leadmeter.ru)

---

## 🔥 Ключевые проекты

### 🧠 AI Catalog Consultant

**AI-консультант по товарному каталогу с контролируемыми LLM tools, structured retrieval и RAG.**

Пользователь задаёт вопрос обычным языком, а система подбирает реальные товары по цене, характеристикам и наличию. LLM не является источником товарных фактов: данные берутся из PostgreSQL и закрытых инструментов.

`Catalog → Python ingestion → PostgreSQL → pgvector → Consultant Core → MCP → n8n → Telegram`

**Что реализовано:**
- ingestion и нормализация реального e-commerce каталога;
- PostgreSQL + pgvector;
- structured SQL retrieval и semantic evidence;
- закрытый набор typed LLM tools вместо произвольного SQL;
- deterministic ranking и semantic guard;
- multi-turn диалог;
- incremental embeddings;
- Telegram + n8n orchestration;
- retrieval/agent evaluation, regression и acceptance tests.

**Стек:** Python · PostgreSQL · pgvector · OpenAI · MCP · n8n · Docker · Telegram

👉 [Код и архитектура](https://github.com/rbabashaikhov/ai-automation-lab/tree/main/projects/ai-catalog-consultant)

---

### 🔐 Enterprise Private GPT

**Полностью локальный RAG-ассистент для работы с юридическими документами без внешнего LLM API.**

`Documents → Chunking → multilingual-e5-small → Qdrant → Relevance Gate → Local LLM → Answer`

**Что реализовано:**
- локальные embeddings и inference;
- Qdrant semantic search;
- relevance threshold для нерелевантных запросов;
- chunking и очистка коротких фрагментов;
- измерение retrieval/generation latency;
- retrieval evaluation;
- локальный запуск через Ollama.

**Стек:** Python · LangChain · Qdrant · multilingual-e5-small · Ollama · Qwen · Docker

👉 [Репозиторий](https://github.com/rbabashaikhov/enterprise-private-gpt)

---

### 📊 SEO Analytics Pipeline

**Python-пайплайн для объединения Google Search Console и Яндекс Вебмастера в единую аналитическую модель для Power BI.**

`GSC + Yandex Webmaster → Python ETL → Validation → Normalization → Analytics layer → Power BI`

**Что реализовано:**
- единый контракт данных для двух поисковых систем;
- нормализация дат, устройств и метрик;
- корректный расчёт CTR и weighted average position;
- data-quality проверки;
- воспроизводимый публичный demo mode без credentials;
- граница интеграции с PostgreSQL;
- Power BI dashboard.

**Стек:** Python · pandas · SQLAlchemy · PostgreSQL · Power BI · pytest · GitHub Actions

👉 [Репозиторий](https://github.com/rbabashaikhov/seo-analytics-pipeline)

---

## ⚙️ AI Automation Lab

Репозиторий с инженерными инструментами и экспериментами вокруг AI/automation.

В том числе — **n8n Workflow-as-Code Tool**: CLI для discovery, export, diff и безопасного обновления n8n workflow через API.

👉 [AI Automation Lab](https://github.com/rbabashaikhov/ai-automation-lab)

---

## 🛠 Основной стек

**AI / LLM:** OpenAI API · RAG · embeddings · pgvector · Qdrant · MCP · tool use · local LLM  
**Backend / Data:** Python · SQL · PostgreSQL · REST API · ETL/ELT · pandas  
**Automation:** n8n · API integrations · Telegram bots  
**Analytics / BI:** Power BI · web/product analytics · data quality  
**Infrastructure:** Docker · Linux · VPS · Git · GitHub Actions

---

## 💡 Как я подхожу к разработке

Мне интересны не просто AI-демо, а системы, которые можно **проверить, измерить, поддерживать и использовать в реальной работе**.

Для AI-проектов я смотрю на весь цикл:

`Data quality → Retrieval → Grounding → Evaluation → Latency → Cost → Reliability → Production`

Для аналитических проектов:

`Sources → Data model → Validation → Transformation → Metrics → BI → Business decision`

---

## 📱 Другие проекты

Telegram Mini Apps, AI-боты, веб-приложения и аналитические сервисы:

👉 [apps.leadmeter.ru](https://apps.leadmeter.ru)

---

## 📬 Связаться

Если вам нужен **AI-ассистент, RAG-система, автоматизация, интеграция данных, аналитический pipeline или BI-решение** — буду рад обсудить задачу.

🌐 [leadmeter.ru](https://leadmeter.ru)
