# Awesome News Provider Connectors

A curated collection of 85 ready-to-use **connectors** for
[news-provider](https://github.com/Leo-RH/news-provider) — the JSON-driven
news aggregation engine and API.

This repository contains **no code**. Each connector is a single JSON file that
tells the news-provider engine how to read one website: which pages (or RSS
feed) to fetch, how to split them into article blocks, and where to find each
field (title, description, date, link, topic, image). The engine itself lives
in the [news-provider](https://github.com/Leo-RH/news-provider) repository.

> These connectors use features of the current news-provider engine (RSS
> connectors, `:self` links, sibling grouping, date languages/time zones,
> per-connector parser). Use an up-to-date engine.

---

## Categories

Connectors are grouped by subject, one folder per category. The folder name
becomes the articles' `category` in the API (`/news?category=games`).

| Folder | Connectors | Description |
|--------|-----------:|-------------|
| [`technology/`](technology/) | 8 | Consumer tech: new devices, computers, phones and gadgets |
| [`it/`](it/) | 5 | Infrastructure, cloud, databases, data and software development |
| [`ai/`](ai/) | 6 | Artificial intelligence news, research and industry |
| [`world/`](world/) | 8 | General and world news |
| [`games/`](games/) | 8 | Video game releases, reviews and industry news |
| [`science/`](science/) | 6 | Science, research and space |
| [`business/`](business/) | 4 | Business, markets and the economy |
| [`open-source/`](open-source/) | 5 | Linux, open-source software and developer platforms |
| [`entertainment/`](entertainment/) | 9 | TV shows, movies and streaming |
| [`music/`](music/) | 9 | New albums, tours, shows and music industry news |
| [`cybersecurity/`](cybersecurity/) | 17 | Cybersecurity news, threat intelligence and vulnerability coverage |

More categories may be added over time.

**Type** is `html` (the site's pages are scraped) or `rss` (the site's official feed is read).

### technology

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `9to5MacConnector.json` | [9to5Mac](https://9to5mac.com) | html | `/` |
| `androidAuthorityConnector.json` | [Android Authority](https://www.androidauthority.com) | rss | `/feed/` |
| `engadgetConnector.json` | [Engadget](https://www.engadget.com) | html | `/` |
| `techCrunchConnector.json` | [TechCrunch](https://techcrunch.com) | html | `/latest/` |
| `tecmundoConnector.json` | [Tecmundo](https://www.estadao.com.br/tecmundo) | html | `/` |
| `tecnoblogConnector.json` | [Tecnoblog](https://tecnoblog.net) | html | `/` |
| `theVergeConnector.json` | [The Verge](https://www.theverge.com) | html | `/tech` |
| `tomsHardwareConnector.json` | [Tom's Hardware](https://www.tomshardware.com) | html | `/news` |

### it

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `computerworldConnector.json` | [Computerworld](https://www.computerworld.com) | html | `/news/` |
| `dbEnginesBlogConnector.json` | [DB-Engines Blog](https://db-engines.com) | html | `/en/blog` |
| `infoQConnector.json` | [InfoQ](https://www.infoq.com) | html | `/news/` |
| `infoWorldConnector.json` | [InfoWorld](https://www.infoworld.com) | html | `/news/` |
| `networkWorldConnector.json` | [Network World](https://www.networkworld.com) | html | `/news/` |

### ai

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `huggingFaceBlogConnector.json` | [Hugging Face Blog](https://huggingface.co) | rss | `/blog/feed.xml` |
| `marktechpostConnector.json` | [MarkTechPost](https://www.marktechpost.com) | html | `/` |
| `mitTechnologyReviewAIConnector.json` | [MIT Technology Review - AI](https://www.technologyreview.com) | rss | `/topic/artificial-intelligence/feed` |
| `techCrunchAIConnector.json` | [TechCrunch - AI](https://techcrunch.com) | html | `/category/artificial-intelligence/` |
| `theDecoderConnector.json` | [The Decoder](https://the-decoder.com) | html | `/` |
| `ventureBeatAIConnector.json` | [VentureBeat - AI](https://venturebeat.com) | html | `/category/ai/` |

### world

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `alJazeeraConnector.json` | [Al Jazeera](https://www.aljazeera.com) | html | `/news/` |
| `bbcNewsBrasilConnector.json` | [BBC News Brasil](https://www.bbc.com) | html | `/portuguese` |
| `bbcNewsWorldConnector.json` | [BBC News - World](https://www.bbc.com) | html | `/news/world` |
| `dwConnector.json` | [DW - Top Stories](https://www.dw.com) | html | `/en/top-stories/s-9097` |
| `financialTimesWorldConnector.json` | [Financial Times - World](https://www.ft.com) | rss | `/world?format=rss` |
| `folhaConnector.json` | [Folha de S.Paulo](https://www1.folha.uol.com.br) | html | `/ultimas-noticias/` |
| `g1Connector.json` | [G1](https://g1.globo.com) | html | `/`, `/mundo/`, `/politica/`, `/economia/` |
| `theGuardianWorldConnector.json` | [The Guardian - World](https://www.theguardian.com) | html | `/world` |

### games

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `eurogamerConnector.json` | [Eurogamer](https://www.eurogamer.net) | html | `/news` |
| `flowGamesConnector.json` | [Flow Games](https://flowgames.gg) | html | `/` |
| `gameSpotConnector.json` | [GameSpot](https://www.gamespot.com) | rss | `/feeds/news/` |
| `ignConnector.json` | [IGN](https://www.ign.com) | html | `/news` |
| `pcGamerConnector.json` | [PC Gamer](https://www.pcgamer.com) | html | `/news/` |
| `polygonConnector.json` | [Polygon](https://www.polygon.com) | html | `/news/` |
| `rockPaperShotgunConnector.json` | [Rock Paper Shotgun](https://www.rockpapershotgun.com) | html | `/news` |
| `voxelConnector.json` | [Voxel](https://www.estadao.com.br/tecmundo/voxel) | rss | official feed |

### science

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `nasaNewsConnector.json` | [NASA News](https://www.nasa.gov) | html | `/news/recently-published/` |
| `newScientistConnector.json` | [New Scientist](https://www.newscientist.com) | html | `/section/news/` |
| `physOrgConnector.json` | [Phys.org](https://phys.org) | html | `/` |
| `scienceDailyConnector.json` | [ScienceDaily](https://www.sciencedaily.com) | html | `/news/top/science/` |
| `scientificAmericanConnector.json` | [Scientific American](https://www.scientificamerican.com) | html | `/latest/` |
| `spaceComConnector.json` | [Space.com](https://www.space.com) | html | `/news` |

### business

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `bbcBusinessConnector.json` | [BBC News - Business](https://www.bbc.com) | html | `/business` |
| `cnbcConnector.json` | [CNBC](https://www.cnbc.com) | html | `/world/` |
| `infoMoneyConnector.json` | [InfoMoney](https://www.infomoney.com.br) | html | `/ultimas-noticias/` |
| `valorEconomicoConnector.json` | [Valor Econômico](https://valor.globo.com) | html | `/ultimas-noticias/` |

### open-source

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `gitHubBlogConnector.json` | [The GitHub Blog](https://github.blog) | html | `/` |
| `itsFossNewsConnector.json` | [It's FOSS News](https://itsfoss.com) | html | `/news/` |
| `lwnConnector.json` | [LWN.net](https://lwn.net) | html | `/` |
| `omgUbuntuConnector.json` | [OMG! Ubuntu](https://www.omgubuntu.co.uk) | html | `/` |
| `phoronixConnector.json` | [Phoronix](https://www.phoronix.com) | rss | `/rss.php` |

### entertainment

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `adoroCinemaConnector.json` | [AdoroCinema](https://www.adorocinema.com) | html | `/` |
| `colliderConnector.json` | [Collider](https://collider.com) | html | `/` |
| `deadlineConnector.json` | [Deadline](https://deadline.com) | html | `/` |
| `hollywoodReporterConnector.json` | [The Hollywood Reporter - TV](https://www.hollywoodreporter.com) | html | `/c/tv/tv-news/` |
| `indieWireConnector.json` | [IndieWire](https://www.indiewire.com) | html | `/c/news/` |
| `omeleteConnector.json` | [Omelete](https://www.omelete.com.br) | html | `/` |
| `pipocaModernaConnector.json` | [Pipoca Moderna](https://pipocamoderna.com.br) | html | `/` |
| `screenRantConnector.json` | [Screen Rant](https://screenrant.com) | html | `/` |
| `varietyTVConnector.json` | [Variety - TV](https://variety.com) | html | `/v/tv/` |

### music

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `billboardConnector.json` | [Billboard](https://www.billboard.com) | html | `/c/music/music-news/` |
| `consequenceConnector.json` | [Consequence](https://consequence.net) | html | `/category/music/` |
| `loudwireConnector.json` | [Loudwire](https://loudwire.com) | html | `/category/news/` |
| `nmeConnector.json` | [NME](https://www.nme.com) | html | `/news/music` |
| `pitchforkConnector.json` | [Pitchfork](https://pitchfork.com) | html | `/news/` |
| `rollingStoneBrasilConnector.json` | [Rolling Stone Brasil](https://rollingstone.com.br) | html | `/` |
| `rollingStoneConnector.json` | [Rolling Stone - Music](https://www.rollingstone.com) | html | `/music/music-news/` |
| `stereogumConnector.json` | [Stereogum](https://www.stereogum.com) | html | `/category/news` |
| `tenhoMaisDiscosQueAmigosConnector.json` | [Tenho Mais Discos Que Amigos!](https://www.tenhomaisdiscosqueamigos.com) | html | `/` |

### cybersecurity

| Connector | Site | Type | Pages / feed |
|-----------|------|------|--------------|
| `arsTechnicaSecurityConnector.json` | [Ars Technica - Security](https://arstechnica.com) | rss | `/security/feed/` |
| `bleepingComputerConnector.json` | [BleepingComputer](https://www.bleepingcomputer.com) | html | `/news/security/` |
| `csoOnlineConnector.json` | [CSO Online](https://www.csoonline.com) | html | `/news/` |
| `cyberScoopConnector.json` | [CyberScoop](https://cyberscoop.com) | html | `/` |
| `darkReadingConnector.json` | [Dark Reading](https://www.darkreading.com) | rss | `/rss.xml` |
| `grahamCluleyConnector.json` | [Graham Cluley](https://grahamcluley.com) | rss | `/feed/` |
| `helpNetSecurityConnector.json` | [Help Net Security](https://www.helpnetsecurity.com) | html | `/` |
| `infosecurityMagazineConnector.json` | [Infosecurity Magazine](https://www.infosecurity-magazine.com) | html | `/news/` |
| `krebsOnSecurityConnector.json` | [Krebs on Security](https://krebsonsecurity.com) | html | `/` |
| `schneierOnSecurityConnector.json` | [Schneier on Security](https://www.schneier.com) | html | `/` |
| `scMediaConnector.json` | [SC Media](https://www.scworld.com) | html | `/news` |
| `securityAffairsConnector.json` | [Security Affairs](https://securityaffairs.com) | html | `/`, `/category/hacking` |
| `securityWeekConnector.json` | [SecurityWeek](https://www.securityweek.com) | html | `/` |
| `theHackerNewsConnector.json` | [The Hacker News](https://thehackernews.com) | html | `/search/label/Threat%20Intelligence`, `/search/label/Vulnerability`, `/search/label/Cyber%20Attack`, `/` |
| `theRecordConnector.json` | [The Record](https://therecord.media) | html | `/` |
| `theRegisterSecurityConnector.json` | [The Register - Security](https://www.theregister.com) | html | `/security/` |
| `wiredSecurityConnector.json` | [WIRED - Security](https://www.wired.com) | html | `/category/security/` |

---

## Usage

1. Set up [news-provider](https://github.com/Leo-RH/news-provider) by following
   its README.
2. Point the engine at this repository. Connectors are found recursively and
   each folder becomes a category:

   ```bash
   CONNECTORS_DIR=/path/to/awesome_news_provider_connectors python main.py
   ```

   Or only one category:

   ```bash
   CONNECTORS_DIR=/path/to/awesome_news_provider_connectors/cybersecurity python main.py
   ```

   You can also copy the folders you want into news-provider's `connectors/`
   directory.

3. Start the API and check the connectors at `http://127.0.0.1:5000/sources`.
   Each one shows a health status (`ok`, `partial`, `empty`, `error`).

---

## Contributing a connector

The full guide to writing connectors is
[`CONNECTORS.md`](https://github.com/Leo-RH/news-provider/blob/main/CONNECTORS.md)
in the news-provider repository. In short:

- One site per JSON file, named `<siteName>Connector.json`.
- Put it in the folder for its category, or create a new category folder.
- If the site has an official RSS/Atom feed, an `rss` connector is the most
  robust choice; scrape the HTML when there is no feed or it lacks content.
- Set `language` (and `timezone`) for sites that don't publish in English, so
  their dates are understood.
- Test it with news-provider before opening a pull request: it should show
  status `ok` in `/sources` and return articles with at least a title and a link.
- Add it to the table in this README.

> Websites change their HTML from time to time. If a connector's status turns
> `empty`, its selectors probably need updating. Issues and pull requests are
> welcome.

---

## License

[MIT](LICENSE)
