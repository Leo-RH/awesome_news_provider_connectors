# Awesome News Provider Connectors

A curated collection of ready-to-use **connectors** for
[news-provider](https://github.com/Leo-RH/news-provider) — the JSON-driven
news aggregation engine and API.

This repository contains **no code**. Each connector is a single JSON file that
tells the news-provider engine how to read one website: which pages to fetch,
how to split them into article blocks, and where to find each field (title,
description, date, link, topic, image). The engine itself lives in the
[news-provider](https://github.com/Leo-RH/news-provider) repository.

---

## Categories

Connectors are grouped by subject, one folder per category.

| Folder | Description |
|--------|-------------|
| [`cybersecurity/`](cybersecurity/) | Cybersecurity news, threat intelligence and vulnerability coverage |

More categories may be added over time.

### cybersecurity

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `bleepingComputerConnector.json` | [BleepingComputer](https://www.bleepingcomputer.com) | `/news/security/` |
| `csoOnlineConnector.json` | [CSO Online](https://www.csoonline.com) | `/news/` |
| `cyberScoopConnector.json` | [CyberScoop](https://cyberscoop.com) | `/` |
| `helpNetSecurityConnector.json` | [Help Net Security](https://www.helpnetsecurity.com) | `/` |
| `infosecurityMagazineConnector.json` | [Infosecurity Magazine](https://www.infosecurity-magazine.com) | `/news/` |
| `krebsOnSecurityConnector.json` | [Krebs on Security](https://krebsonsecurity.com) | `/` |
| `scMediaConnector.json` | [SC Media](https://www.scworld.com) | `/news` |
| `schneierOnSecurityConnector.json` | [Schneier on Security](https://www.schneier.com) | `/` |
| `securityAffairsConnector.json` | [Security Affairs](https://securityaffairs.com) | `/`, `/category/hacking` |
| `securityWeekConnector.json` | [SecurityWeek](https://www.securityweek.com) | `/` |
| `theHackerNewsConnector.json` | [The Hacker News](https://thehackernews.com) | `/`, `/search/label/Threat%20Intelligence`, `/search/label/Vulnerability`, `/search/label/Cyber%20Attack` |
| `theRegisterSecurityConnector.json` | [The Register](https://www.theregister.com) | `/security/` |
| `wiredSecurityConnector.json` | [WIRED](https://www.wired.com) | `/category/security/` |

---

## Usage

1. Set up [news-provider](https://github.com/Leo-RH/news-provider) by following
   its README.
2. Copy the connectors you want into news-provider's `connectors/` directory:

   ```bash
   cp cybersecurity/*.json /path/to/news-provider/connectors/
   ```

   Or point the engine straight at a category folder of this repo with the
   `CONNECTORS_DIR` environment variable:

   ```bash
   CONNECTORS_DIR=/path/to/awesome_news_provider_connectors/cybersecurity python main.py
   ```

3. Start the API and check the connectors loaded at
   `http://127.0.0.1:5000/sources`.

---

## Contributing a connector

The full guide to writing connectors is
[`CONNECTORS.md`](https://github.com/Leo-RH/news-provider/blob/main/CONNECTORS.md)
in the news-provider repository. In short:

- One site per JSON file, named `<siteName>Connector.json`.
- Put it in the folder for its category, or create a new category folder.
- Test it with news-provider before opening a pull request. It should return
  articles with at least a title and a link.
- Add it to the table in this README.

> Websites change their HTML from time to time. If a connector stops
> returning articles, its selectors probably need updating. Issues and pull
> requests are welcome.

---

## License

[MIT](LICENSE)
