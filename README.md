# Hi, I'm Vladyslav 👋

I'm a Computing student at TU Dublin, building practical experience through software projects and hands-on learning. My interests include Python development, computer vision, and local AI tools.

## What I'm working on

- building computer vision tools for custom object detection
- connecting local language models to practical tools
- strengthening my software-engineering fundamentals through readable code, testing, and clear documentation

## Selected work

### PracticeLoop · [Live demo](https://practiceloop.pages.dev)

A maths practice web app, built with a second developer: users pick a topic and difficulty, get a generated problem, type their answer in a maths editor, and can reveal the correct answer or a full worked solution, with a history of everything they have solved. Problems are generated from rule-based templates, not by an LLM: every problem has a short shareable code, and a frozen SHA-256-based PRNG makes the same code always reproduce the same problem. A catalogue of 14,080 problems across 50 topics (algebra, calculus, probability and statistics) is built and checked with SymPy at deploy time. Answers are graded by SymPy symbolic equivalence in a sandboxed worker with CPU and memory limits, so any mathematically equal form is accepted. The project also generates PDF worksheets and 3D graphs for multivariable integrals, and is covered by about 8,000 automated tests. *The repository is private.*

**Built with:** Python, FastAPI, SymPy, PostgreSQL (Supabase, row-level security), React, TypeScript, Vite, KaTeX, MathLive, Three.js, Cloudflare Pages, GitHub Actions.

### [Bullseye](https://github.com/whatvlad/bullseye-lab)

A real-time market data analytics system. It ingests a live stream of market events over WebSocket/RPC, detects signals, and validates strategies through paper trading with no real money. Latency and API rate limits are handled so that all data collection stays within a free API tier. Data is stored in PostgreSQL, and strategies are checked with backtests, replay analysis, and out-of-sample validation on a dataset of 80k+ observations. A Telegram bot provides control (start/stop, settings, alerts), and the project is covered by 600+ automated tests.

**Built with:** Python, asyncio, WebSockets, PostgreSQL, SQLAlchemy, Alembic, Docker, Telegram Bot API, pytest.

### [Custom Object Detection](https://github.com/whatvlad/custom-object-detection)

A configurable single-class object detection pipeline for game screenshots. It includes screenshot collection, a mouse-based annotation tool, YOLO training, and live bounding-box predictions in a preview window or an optional Windows overlay. A synthetic dataset generator is included for trying the pipeline before collecting gameplay images.

**Built with:** Python, Ultralytics YOLO, OpenCV, MSS, NumPy.

### [Local AI Agent](https://github.com/whatvlad/local-ai-agent)

A local Ollama assistant with a Telegram interface and Python tools for web research, persistent reminders, and email. Model-generated tool requests are routed to explicit functions, with tool errors returned to the model for correction. SQLite stores reminders and email drafts; reviewed drafts can be sent through SMTP, and inbox messages can be read through IMAP.

**Built with:** Python, Ollama, python-telegram-bot, SQLite, HTTPX, DDGS, SMTP/IMAP.

### [Python Utilities](https://github.com/whatvlad/pyprojects)

A small collection of practical command-line tools, including a password generator, configurable port scanner, and WHOIS client. The project includes safer defaults, usage documentation, and automated Python checks.

## Technologies

- **Languages:** Python, Java, JavaScript, C, C++
- **Computer vision:** Ultralytics YOLO, OpenCV, NumPy
- **AI and automation:** Ollama, Telegram bots, Python tool calling
- **Web:** HTML, CSS, responsive layouts
- **Data and tools:** PostgreSQL, SQLite, Docker, Git, GitHub Actions, pytest

## Learning in public

My older exercise repositories remain public and are clearly marked as learning archives. They document the path from early programming and web-development exercises to larger, better-structured projects.

I'm currently focused on turning that foundation into complete projects with readable code, useful documentation, and reproducible setup.
