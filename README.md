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
| [`technology/`](technology/) | Consumer tech: new devices, computers, phones and gadgets |
| [`it/`](it/) | Infrastructure, cloud, databases, data and software development |
| [`ai/`](ai/) | Artificial intelligence news, research and industry |
| [`world/`](world/) | General and world news |
| [`games/`](games/) | Video game releases, reviews and industry news |
| [`science/`](science/) | Science, research and space |
| [`business/`](business/) | Business, markets and the economy |
| [`open-source/`](open-source/) | Linux, open-source software and developer platforms |
| [`entertainment/`](entertainment/) | TV shows, movies and streaming |
| [`music/`](music/) | New albums, tours, shows and music industry news |
| [`cybersecurity/`](cybersecurity/) | Cybersecurity news, threat intelligence and vulnerability coverage |

More categories may be added over time.

### technology

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `9to5MacConnector.json` | [9to5Mac](https://9to5mac.com) | `/` |
| `engadgetConnector.json` | [Engadget](https://www.engadget.com) | `/` |
| `techCrunchConnector.json` | [TechCrunch](https://techcrunch.com) | `/latest/` |
| `tecmundoConnector.json` | [Tecmundo](https://www.estadao.com.br/tecmundo) | `/` |
| `tecnoblogConnector.json` | [Tecnoblog](https://tecnoblog.net) | `/` |
| `theVergeConnector.json` | [The Verge](https://www.theverge.com) | `/tech` |
| `tomsHardwareConnector.json` | [Tom's Hardware](https://www.tomshardware.com) | `/news` |

### it

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `computerworldConnector.json` | [Computerworld](https://www.computerworld.com) | `/news/` |
| `dbEnginesBlogConnector.json` | [DB-Engines Blog](https://db-engines.com) | `/en/blog` |
| `infoQConnector.json` | [InfoQ](https://www.infoq.com) | `/news/` |
| `infoWorldConnector.json` | [InfoWorld](https://www.infoworld.com) | `/news/` |

### ai

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `marktechpostConnector.json` | [MarkTechPost](https://www.marktechpost.com) | `/` |
| `techCrunchAIConnector.json` | [TechCrunch - AI](https://techcrunch.com) | `/category/artificial-intelligence/` |
| `theDecoderConnector.json` | [The Decoder](https://the-decoder.com) | `/` |
| `ventureBeatAIConnector.json` | [VentureBeat - AI](https://venturebeat.com) | `/category/ai/` |

### world

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `alJazeeraConnector.json` | [Al Jazeera](https://www.aljazeera.com) | `/news/` |
| `bbcNewsBrasilConnector.json` | [BBC News Brasil](https://www.bbc.com) | `/portuguese` |
| `bbcNewsWorldConnector.json` | [BBC News - World](https://www.bbc.com) | `/news/world` |
| `dwConnector.json` | [DW - Top Stories](https://www.dw.com) | `/en/top-stories/s-9097` |
| `g1Connector.json` | [G1](https://g1.globo.com) | `/`, `/mundo/`, `/politica/`, `/economia/` |
| `theGuardianWorldConnector.json` | [The Guardian - World](https://www.theguardian.com) | `/world` |

### games

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `eurogamerConnector.json` | [Eurogamer](https://www.eurogamer.net) | `/news` |
| `flowGamesConnector.json` | [Flow Games](https://flowgames.gg) | `/` |
| `ignConnector.json` | [IGN](https://www.ign.com) | `/news` |
| `pcGamerConnector.json` | [PC Gamer](https://www.pcgamer.com) | `/news/` |
| `polygonConnector.json` | [Polygon](https://www.polygon.com) | `/news/` |
| `rockPaperShotgunConnector.json` | [Rock Paper Shotgun](https://www.rockpapershotgun.com) | `/news` |

### science

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `nasaNewsConnector.json` | [NASA News](https://www.nasa.gov) | `/news/recently-published/` |
| `physOrgConnector.json` | [Phys.org](https://phys.org) | `/` |
| `scientificAmericanConnector.json` | [Scientific American](https://www.scientificamerican.com) | `/latest/` |
| `spaceComConnector.json` | [Space.com](https://www.space.com) | `/news` |

### business

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `bbcBusinessConnector.json` | [BBC News - Business](https://www.bbc.com) | `/business` |
| `cnbcConnector.json` | [CNBC](https://www.cnbc.com) | `/world/` |
| `infoMoneyConnector.json` | [InfoMoney](https://www.infomoney.com.br) | `/ultimas-noticias/` |
| `valorEconomicoConnector.json` | [Valor Econômico](https://valor.globo.com) | `/ultimas-noticias/` |

### open-source

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `gitHubBlogConnector.json` | [The GitHub Blog](https://github.blog) | `/` |
| `itsFossNewsConnector.json` | [It's FOSS News](https://itsfoss.com) | `/news/` |
| `omgUbuntuConnector.json` | [OMG! Ubuntu](https://www.omgubuntu.co.uk) | `/` |

### entertainment

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `adoroCinemaConnector.json` | [AdoroCinema](https://www.adorocinema.com) | `/` |
| `colliderConnector.json` | [Collider](https://collider.com) | `/` |
| `deadlineConnector.json` | [Deadline](https://deadline.com) | `/` |
| `hollywoodReporterConnector.json` | [The Hollywood Reporter - TV](https://www.hollywoodreporter.com) | `/c/tv/tv-news/` |
| `indieWireConnector.json` | [IndieWire](https://www.indiewire.com) | `/c/news/` |
| `omeleteConnector.json` | [Omelete](https://www.omelete.com.br) | `/` |
| `pipocaModernaConnector.json` | [Pipoca Moderna](https://pipocamoderna.com.br) | `/` |
| `screenRantConnector.json` | [Screen Rant](https://screenrant.com) | `/` |
| `varietyTVConnector.json` | [Variety - TV](https://variety.com) | `/v/tv/` |

### music

| Connector | Site | Pages crawled |
|-----------|------|---------------|
| `billboardConnector.json` | [Billboard](https://www.billboard.com) | `/c/music/music-news/` |
| `consequenceConnector.json` | [Consequence](https://consequence.net) | `/category/music/` |
| `loudwireConnector.json` | [Loudwire](https://loudwire.com) | `/category/news/` |
| `nmeConnector.json` | [NME](https://www.nme.com) | `/news/music` |
| `pitchforkConnector.json` | [Pitchfork](https://pitchfork.com) | `/news/` |
| `rollingStoneBrasilConnector.json` | [Rolling Stone Brasil](https://rollingstone.com.br) | `/` |
| `rollingStoneConnector.json` | [Rolling Stone - Music](https://www.rollingstone.com) | `/music/music-news/` |
| `stereogumConnector.json` | [Stereogum](https://www.stereogum.com) | `/category/news` |
| `tenhoMaisDiscosQueAmigosConnector.json` | [Tenho Mais Discos Que Amigos!](https://www.tenhomaisdiscosqueamigos.com) | `/` |

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
   cp */*.json /path/to/news-provider/connectors/   # or every category at once
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
