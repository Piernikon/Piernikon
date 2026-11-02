# Mateusz Piernikarczyk (`@Piernikon`)

**Digital & AI Operations Product Manager · AI Agent Orchestration · Process Automation · Hardware Maker**  
📍 Gdańsk / Trójmiasto, Poland · 🔗 [LinkedIn](https://linkedin.com/in/mateusz-piernikarczyk) · 🎥 [Prelekcje o Claude Code (YouTube)](https://www.youtube.com/watch?v=kceI20-zWls)

---

### O mnie / About Me

Projektuję i wdrażam **systemy agentowe AI** oraz **automatyzacje procesów biznesowych i produktowych** - od architektury baz wiedzy kompilowanych przez LLM i strażników jakości w CI/CD, przez integracje e-commerce/CRM/LMS, aż po fizyczne urządzenia IoT (ESP32 + e-paper + parametryczny CAD).

I design and ship **production AI agentic workflows** and **business process automations** - spanning deterministic CI/CD quality guards for LLM agents, compiled Markdown knowledge bases, end-to-end API/no-code pipelines, and embedded hardware projects (ESP32 + e-Paper + Python CAD).

---

### Wybrane projekty publiczne / Featured Public Repositories

| Repozytorium / Repository | Zakres i architektura / Scope & Architecture | Stack |
|---|---|---|
| **[`llm-wiki-toolkit`](https://github.com/Piernikon/llm-wiki-toolkit)** | **Deterministic Guardrails & Hybrid FTS5 Search for Agentic Knowledge Bases.** Zestaw narzędzi Python/SQLite do utrzymywania bazy wiedzy w architekturze *LLM Wiki* (inspirowanej koncepcją [Andrej Karpathy - LLM Wiki](https://x.com/karpathy)): dwuwarstwowa wyszukiwarka **SQLite FTS5 + BM25/stemming**, strażnik pre-commit weryfikujący **pochodzenie głosu (`głos:`)**, chronologię decyzji i integralność linków, auto-kompilator indeksów oraz lekka kolejka **Anthropic Message Batches API (-50% kosztu, 0 tokenów kontekstu)**. | `Python 3.11+` · `SQLite FTS5` · `Anthropic Batch API` · `Git Hooks` · `Obsidian` |
| **[`epaper-storm-station`](https://github.com/Piernikon/epaper-storm-station)** | **7.5" e-Paper Outdoor Storm Warning & Indoor Weather Station (ESP32 + Parametric CAD).** Rozbudowany układ i logika dla stacji pogodowej z dwuczynnikowym alarmem wichurowym (wiatr stały + porywy z histerezą), 3-godzinnym trendem barycznym w pamięci RTC, analizą punktu rosy i opłacalności wietrzenia (Magnus-Tetens), klasyfikacją pyłków CAMS, testami natywnymi (`pio test -e native`) oraz parametryczną obudową 3D w Pythonie (`build123d`). | `C++17` · `ESP32` · `PlatformIO` · `Unity Tests` · `build123d (CAD)` · `SVG` |

---

### Obszary specjalizacji / Core Domains

- **AI Agent Engineering & Governance:** Orkiestracja wieloagentowa (Claude Code, Gemini, Codex, [Hermes Agent](https://github.com/NousResearch/hermes-agent)), deterministyczne strażniki jakości (pre-commit / GitHub Actions), architektura pojedynczego pisarza (*single-writer pattern*), optymalizacja kosztów tokenów (Batch API, lokalne indeksy SQLite FTS5 zamiast pełnego skanowania kontekstu).
- **Digital Product & Operations:** Zarządzanie ekosystemem webowym (Astro, WordPress/WooCommerce, Kajabi), automatyzacja przepływów CRM/sprzedaży/obsługi (Zapier, n8n, Google Apps Script, REST API, Webhooks), analityka produktowa i konwersji (GA4, GTM, Microsoft Clarity, Looker Studio).
- **Hardware & Maker Workshop:** Mikrokontrolery ESP32 (deep-sleep ~14 µA, e-paper Waveshare, I2C BME280/BME688), modelowanie parametryczne CAD w kodzie (`build123d` -> STEP/STL) oraz druk 3D (PETG / TPU).

---

### Prelekcje i wystąpienia / Public Talks (PL)

- 🎥 [**Claude Code w praktyce - jak budować i utrzymywać produkty z agentami AI (Część 1)**](https://www.youtube.com/watch?v=kceI20-zWls)
- 🎥 [**Claude Code - architektura skilli, strażników jakości i automatyzacji (Część 2)**](https://www.youtube.com/watch?v=Fdb4kln1-mA)

---

### Podziękowania i inspiracje / Credits & Upstream Inspirations

Moje rozwiązania open-source stoją na ramionach świetnych projektów społeczności:
- **[Andrej Karpathy](https://github.com/karpathy)** - za koncepcję *LLM Wiki* (kompilowanie źródeł do połączonych stron Markdown przez agenta zamiast klasycznego RAG-a tylko do odczytu) oraz ideę dopasowanego mikro-oprogramowania.
- **[Luke Marzen (`lmarzen/esp32-weather-epd`)](https://github.com/lmarzen/esp32-weather-epd)** oraz **[`lumixen/esp32-weather-epd`](https://github.com/lumixen/esp32-weather-epd)** - za fundament oprogramowania dla wyświetlaczy e-paper 7.5" i integrację z Open-Meteo (licencja GPLv3).
- **[`gumyr/build123d`](https://github.com/gumyr/build123d)** oraz autorzy projektów obudów na Printables (**FrAllard**, **boriss3D**) - za fundamenty parametrycznego CAD w Pythonie i inspiracje konstrukcyjne dla stacji pogodowej.
- **[Anthropic (`anthropics`)](https://github.com/anthropics)** & **[Nous Research (`NousResearch/hermes-agent`)](https://github.com/NousResearch/hermes-agent)** - za wzorce bezpieczeństwa agentów, strukturę skilli (`SKILL.md`) i narzędzia ekosystemu Claude.
