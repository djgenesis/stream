# "Stream app" Configuration Templates

This repository contains a fully optimized collection of configuration templates and formatting files for the following:
   - **AIOStreams (two different formatters according to if you want to show badges or not**
   - **AIOMetadata**
   - **CutomFusionBadges**

It is designed to deliver premium quality stream results with rich metadata, offering two distinct visual setups (with or without custom badges).

---

## 📋 Prerequisites

Before starting the setup process, ensure you have the following:
1. **Downloaded and installed your "Stream app"** on your mobile and TV (preferably Android /Google TV).
2. **Registered and loged in** in your favorite "Streaming app" website as well as in the apps themselves.
1. **An active Debrid Subscription** (e.g., RealDebrid, AllDebrid, Premiumize, etc.).
2. **Accounts and API Keys** for the metadata and layout services. You will need to input your own keys in the configuration from these platforms:
   - [`"gemini"`](https://ai.google.dev/) (Google Gemini API)
   - [`"openrouter"`](https://openrouter.ai/) (OpenRouter API)
   - [`"tmdb"`](https://www.themoviedb.org/) (The Movie Database)
   - [`"tvdb"`](https://thetvdb.com/) (The TVDB)
   - [`"fanart"`](https://fanart.tv/) (Fanart.tv)
   - [`"rpdb"`](https://ratingposterdb.com/) (Rating Poster Database)
   - [`"topPoster"`](https://topposter.com/)
   - [`"mdblist"`](https://mdblist.com/) (MdbList)
   - [`"traktTokenId"`](https://trakt.tv/) (Trakt.tv)
   - [`"simklTokenId"`](https://simkl.com/) (Simkl)
   - [`"anilistTokenId"`](https://anilist.co/) (AniList)
   - *...any other required provider api keys.*
3. **Select your addon instance(s)** and track their real-time uptime status here: [IbbyLabs Uptime](https://uptime.ibbylabs.dev/).

⚠️ **Important Infrastructure Advice:** For optimal performance and system stability, it is highly recommended to use **only one instance for AIOMetadata** and **one instance for AIOStreams** (or a single secondary instance strictly as a backup).

---

## 🛠️ Repository File Structure

The repository includes the following essential template files:
- [`aiometadata-config.json`](https://github.com/djgenesis/stream/blob/main/aiometadata-config.json) – Master configuration for the AIOMetadata addon.
- [`aiostreams-config.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-config.json) – Base configuration for the AIOStreams addon.
- [`aiostreams-template.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-template.json) – Core template layout for media streams.
- [`gold_badges_complete.json`](https://github.com/djgenesis/stream/blob/main/gold_badges_complete.json) – A comprehensive custom gold badges layout for resolution, audio formats, and video codecs.
- [`formatter-title-usingbadges.json`](https://github.com/djgenesis/stream/blob/main/formatter-title-usingbadges.json) – Stream title formatting optimized for visual badges.
- [`formatter-description-usingbadges.json`](https://github.com/djgenesis/stream/blob/main/formatter-description-usingbadges.json) – Stream description formatting optimized for visual badges.
- [`formatter-title-notusingbadges.json`](https://github.com/djgenesis/stream/blob/main/formatter-title-notusingbadges.json) – Plain text stream title formatting. *(Note: Formed by renaming `title-full.json`)*.
- [`formatter-description-notusingbadges.json`](https://github.com/djgenesis/stream/blob/main/formatter-description-notusingbadges.json) – Plain text stream description formatting.

---

## 🚀 Step-by-Step Setup Guide

Preferably do all the steps on your Android mobile phone. You can choose between **two different paths** depending on your visual preference for your stream layout:

### 🔹 Route A: Using Badges (RECOMENDED Visual Setup)
This path provides a rich graphical experience using clean icons and gold badges for stream resolutions, formats, and audio attributes.
1. Open the configuration page of your chosen **AIOStreams** instance (pick a high-uptime instance from [IbbyLabs Uptime](https://uptime.ibbylabs.dev/)).
2. Download on your device and then upload in the Import section the [`aiostreams-config.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-config.json) or [`aiostreams-template.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-template.json) file.
3. Generate and fill out all your personalized API keys in their respective setup fields.
4. Save and generate your installation link and add it to the "Stream app".
5. Copy the raw url of [`gold_badges_complete.json`](https://raw.githubusercontent.com/djgenesis/stream/refs/heads/main/gold_badges_complete.json) and paste it into the **Custom Badges** in the settings of the "Stream app".

### 🔹 Route B: Not Using Badges (Text Only Setup)
This path provides a classic, distraction-free text format for users who prefer standard text strings over graphical badges.
1. Open the configuration page of your chosen **AIOStreams** instance (pick a high-uptime instance from [IbbyLabs Uptime](https://uptime.ibbylabs.dev/)).
2. Download on your device and then upload in the Import section the [`aiostreams-config.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-config.json) or [`aiostreams-template.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-template.json) file.
3. In the **Formatter** settings, **REPLACE** the contents (copy and paste the contents of [`formatter-title-notusingbadges.json`](https://github.com/djgenesis/stream/blob/main/formatter-title-notusingbadges.json) into the Title section, and [`formatter-description-notusingbadges.json`](https://github.com/djgenesis/stream/blob/main/formatter-description-notusingbadges.json) into the Description section).
4. Generate and fill out all your personalized API keys in their respective setup fields.
5. Save and generate your installation link and add it to the "Stream app".

### 🎬 Configuring AIOMetadata
Regardless of the stream route chosen above, you must configure your metadata catalogs:
1. Open the configuration page for your chosen **AIOMetadata** instance (pick a high-uptime instance from [IbbyLabs Uptime](https://uptime.ibbylabs.dev/)).
2. Download on your device and then upload in the Import section the [`aiometadata-config.json`](https://github.com/djgenesis/stream/blob/main/aiometadata-config.json) file.
3. Generate and fill out all your personalized API keys in their respective setup fields.
4. Save and generate the installation link and add it to "Stream app".

---

## 📁 Included Movie & Series Catalogs

By importing the [`aiometadata-config.json`](https://github.com/djgenesis/stream/blob/main/aiometadata-config.json) profile, the following dynamic metadata catalogs will be automatically integrated into your "Stream app" library interface:

### 🎬 Movies Lists
* **-Trakt Watchlist**
* **Movies Recommended for you**
* **[New Streaming Releases: Movies](https://mdblist.com/lists/snoak/latest-movies-digital-release)**
* **[Latest 4K Movies](https://mdblist.com/lists/maniac2021/latest-4k-releases)**
* **[In Cinemas Now](https://mdblist.com/lists/24hz/in-theatres)**
* **[Trending Movies on Trakt](https://mdblist.com/lists/snoak/trending-movies)**
* **[Top Movies of the Month](https://mdblist.com/lists/antonio0101/top-movies-of-the-week)**
* **[Top 100 Classic Movies](https://trakt.tv/lists/11632963)**
* **[Top Action Movies](https://mdblist.com/lists/hdlists/latest-hd-action-movies-from-1980-to-today)**
* **[New Action Releases](https://mdblist.com/lists/snoak/latest-action-movies)**
* **[Modern Action](https://letterboxd.com/sisamim/list/modern-action/)**
* **[Action Movies (2000 - 2020)](https://trakt.tv/lists/11255166)**
* **[Top 10 Action Movies Of 21st Century](https://trakt.tv/lists/4297336)**
* **[Top Comedy Movies](https://mdblist.com/lists/hdlists/comedy-movies-2001-2020)**
* **[New Releases in Comedy](https://mdblist.com/lists/snoak/latest-comedy-movies)**
* **[Stand-ups](https://mdblist.com/lists/notamongo5/stand-up-comedy)**
* **[Popular Thriller Movies](https://mdblist.com/lists/snoak/thriller-movies)**
* **[New Thriller Releases](https://mdblist.com/lists/snoak/latest-thriller-movies)**
* **[Psychological Thriller](https://mdblist.com/lists/rizreflects/psychological-thrillers)**
* **[IMDb's Top Thriller Movies](https://trakt.tv/lists/22847415)**
* **[Top Horror Movies](https://mdblist.com/lists/hdlists/latest-hd-horror-movies-top-rated-from-1980-to-today)**
* **[New Horror Releases](https://mdblist.com/lists/snoak/latest-horror-movies)**
* **[Rotten Tomatoes: Best Horror Movies Of All Time](https://trakt.tv/lists/4203408)**
* **[Top Fantasy/Sci-Fi Movies](https://mdblist.com/lists/hdlists/latest-hd-fantasy-sci-fi-movies-top-rated-from-1980-to-today)**
* **[Popular Romance Movies](https://mdblist.com/lists/snoak/popular-romance-movies)**
* **[Best of Romance](https://mdblist.com/lists/rjchignell/best-of-romance)**
* **[Forbidden Love in Movies](https://trakt.tv/lists/11142103)**
* **[IMDb's Top Romance Movies](https://trakt.tv/lists/22847343)**
* **[Popular Animation Movies](https://mdblist.com/lists/snoak/animationanime-movies)**
* **[IMDb's Top Animation Movies](https://trakt.tv/lists/22847039)**
* **[Japanese Anime Movies](https://trakt.tv/lists/23471533)**
* **[Shrek Collection](https://letterboxd.com/fantic/list/shrek/)**
* **[Robert De Niro](https://mdblist.com/lists/mokono/robert-de-niro)**
* **[Al Pacino](https://mdblist.com/lists/mokono/al-pacino)**
* **[Anthony Hopkins](https://mdblist.com/lists/mokono/anthony-hopkins)**
* **[Morgan Freeman](https://mdblist.com/lists/mokono/morgan-freeman)**
* **[Daniel Day-Lewis](https://letterboxd.com/fernanp_23/list/daniel-day-lewis/)**
* **[Christian Bale](https://mdblist.com/lists/mokono/christian-bale)**
* **[Jake Gyllenhaal](https://mdblist.com/lists/andyjacoo/jake-gyllenhaal-2kin4hpskb)**
* **[Ryan Gosling](https://mdblist.com/lists/billryan/ryan-gosling-films)**
* **[Margot Robbie](https://mdblist.com/lists/itsall4meplease/margot-robbie)**
* **[Natalie Portman](https://mdblist.com/lists/reachingout/natalie-portman-month)**
* **[Timothée Chalamet](https://mdblist.com/lists/nobnobz/actor-timoth%C3%A9e-chalamet-1dy5dcud8e)**
* **[Joaquin Phoenix](https://mdblist.com/lists/mokono/joaquin-phoenix)**
* **[Florence Pugh](https://mdblist.com/lists/nobnobz/actor-florence-pugh-t50c8h9o4g)**
* **[Scarlett Johansson](https://mdblist.com/lists/caballitopalo/scarlett-johanssons-movies)**
* **[Cate Blanchett](https://mdblist.com/lists/jossbosses/cate-blanchett)**
* **[Emma Stone](https://mdblist.com/lists/billryan/emma-stone-films)**
* **[Peter Sellers](https://mdblist.com/lists/billryan/peter-sellers-films)**
* **[Leonardo Dicaprio](https://mdblist.com/lists/mokono/leonardo-dicaprio-movies)**
* **[Mark Wahlberg](https://mdblist.com/lists/mokono/mark-wahlberg)**
* **[Tom Hanks](https://mdblist.com/lists/mokono/tom-hanks)**
* **[Denzel Washington](https://mdblist.com/lists/mokono/denzel-washington)**
* **[Michael Caine](https://mdblist.com/lists/mokono/michael-caine)**
* **[James Stewart](https://mdblist.com/lists/mokono/james-stewart)**
* **[Robin Williams](https://mdblist.com/lists/mokono/robin-williams)**
* **[Robert Duvall](https://mdblist.com/lists/mokono/robert-duvall)**
* **[Jeff Bridges](https://mdblist.com/lists/mokono/jeff-bridges)**
* **[Clint Eastwood](https://mdblist.com/lists/mokono/clint-eastwood)**
* **[Gene Hackman](https://mdblist.com/lists/mokono/gene-hackman)**
* **[Philip Seymour Hoffman](https://mdblist.com/lists/mokono/philip-seymour-hoffman)**
* **[Russell Crowe](https://mdblist.com/lists/mokono/russell-crowe)**
* **[Tommy Lee Jones](https://mdblist.com/lists/mokono/tommy-lee-jones)**
* **[Sean Connery](https://mdblist.com/lists/mokono/sean-connery)**
* **[Chistopher Walken](https://mdblist.com/lists/mokono/chistopher-walken)**
* **[Joe Pesci](https://mdblist.com/lists/mokono/joe-pesci)**
* **[Jon Voight](https://mdblist.com/lists/mokono/jon-voight)**
* **[Heath Ledger](https://mdblist.com/lists/mokono/heath-ledger)**
* **[Johnny Depp](https://mdblist.com/lists/mokono/johnny-depp)**
* **[Matthew McConaughey](https://mdblist.com/lists/mokono/matthew-mcconaughey)**
* **[Edward Norton](https://mdblist.com/lists/mokono/edward-norton)**
* **[Brad Pitt](https://mdblist.com/lists/mokono/brad-pitt)**
* **[Matt Damon](https://mdblist.com/lists/mokono/matt-damon)**
* **[Hugh Jackman](https://mdblist.com/lists/mokono/hugh-jackman)**
* **[Robert Downey Jr](https://mdblist.com/lists/mokono/robert-downey-jr)**
* **[Liam Neeson](https://mdblist.com/lists/mokono/liam-neeson)**
* **[Mel Gibson](https://mdblist.com/lists/mokono/mel-gibson)**
* **[Bill Murray](https://mdblist.com/lists/mokono/bill-murray)**
* **[Samuel L Jackson](https://mdblist.com/lists/mokono/samuel-l-jackson)**
* **[Jim Carrey](https://mdblist.com/lists/mokono/jim-carrey)**
* **[Will Smith](https://mdblist.com/lists/mokono/will-smith)**
* **[John Goodman](https://mdblist.com/lists/mokono/john-goodman)**
* **[Bruce Willis](https://mdblist.com/lists/mokono/bruce-willis)**
* **[Director: Nolan](https://letterboxd.com/discovery_17/list/nolan/)**
* **[Argentinian Movies](https://mdblist.com/lists/mxtrakttv/argentina-movies)**
* **[Introduction to French Cinema](https://mdblist.com/lists/roskoe88/intro-to-french-cinema)**
* **[French Movies](https://mdblist.com/lists/jarvis-13128907/france-movies)**
* **[Latest French Cinema](https://mdblist.com/lists/factoor/latest-french-cinema)**
* **[Recommended Korean Movies](https://mdblist.com/lists/molemovies/recommended-korean-cinema)**
* **[Korean Movies](https://mdblist.com/lists/narmeian/korean-cinema)**
* **[Popular Korean Movies](https://mdblist.com/lists/an-kah/popular-korean-movies)**
* **[Spanish Movies](https://mdblist.com/lists/ftor327/spain-movies)**
* **[Popular Spanish Movies](https://mdblist.com/lists/snafuki/spain-popular-movies)**
* **[Introduction to Italian Cinema](https://letterboxd.com/richardjduffy/list/italian-cinema/)**
* **[Italian Movies](https://letterboxd.com/murraldo/list/italian-movies-1/)**
* **[Introduction to Japanese Cinema](https://letterboxd.com/tomodachi/list/intro-to-japanese-film-history/)**
* **[Japanese Movies](https://mdblist.com/lists/jarvis-15299542/japanese-cinema)**
* **[UK Movies](https://mdblist.com/lists/andemer/latest-streaming-movies)**
* **[Latest UK Movies](https://mdblist.com/lists/amything/latest-uk-movies)**
* **[Introduction to German Cinema](https://letterboxd.com/nvdw/list/germany-cinema-around-the-world/)**
* **[German Movies](https://mdblist.com/lists/itsdrewy97/germany)**
* **[Introduction to Mexican Cinema](https://letterboxd.com/dawnofthedead/list/mexican-cinema/)**
* **[Top Mexican Movies](https://letterboxd.com/official/list/top-250-mexican-films/)**
* **[More Mexican Movies](https://letterboxd.com/kon0787/list/mexican-movies/)**
* **[Introduction to Brazilian Cinema](https://letterboxd.com/coffeejazzlofi/list/an-introduction-to-brazilian-film-history/)**
* **[Brazilian Movies](https://mdblist.com/lists/biracosme/brazilian-movies)**
* **[Introduction to Indian Cinema](https://letterboxd.com/mithras_/list/bollywood-essentials-and-my-intro-to-indian/)**
* **[Indian Movies](https://letterboxd.com/mcl/list/indian-cinema/)**
* **[Best Picture Winners](https://letterboxd.com/thaais/list/oscar/)**
* **[Best Actress Winners](https://letterboxd.com/thaais/list/actress-in-a-leading-role/)**
* **[Best Actor Winners](https://letterboxd.com/thaais/list/actor-in-a-leading-role/)**
* **[Best Director Winners](https://letterboxd.com/thaais/list/director/)**
* **[Best Original Song Winners](https://letterboxd.com/thaais/list/original-song/)**
* **[Best International Film Winners](https://letterboxd.com/thaais/list/international-feature/)**
* **[Best Sound Winners](https://letterboxd.com/thaais/list/sound/)**
* **[Best Documentary Winners](https://letterboxd.com/thaais/list/documentary-feature/)**
* **[Best Visual Effects Winners](https://letterboxd.com/thaais/list/visual-effects/)**
* **[Cannes Winners](https://letterboxd.com/lukas1999/list/cannes/)**
* **[Venice Festival Winners](https://mdblist.com/lists/atalante421/venice-film-festival-winners)**
* **[BAFTA Winners](https://letterboxd.com/jacquard/list/bafta/)**
* **[Golden Globe Winners](https://mdblist.com/lists/nobnob/collection-golden-globes-winners)**
* **[2026 Golden Globe Nominees](https://mdblist.com/lists/bsm-venger/golden-globes-2026-nominees)**
* **[1960s Movies](https://mdblist.com/lists/ryankeast/movies-decades-1960s-4oulwbhwix)**
* **[1970s Movies](https://mdblist.com/lists/ryankeast/movies-decades-1970s)**
* **[Best of the 1970s](https://mdblist.com/lists/rjchignell/best-of-the-1970-s)**
* **[1980s Movies](https://mdblist.com/lists/ryankeast/movies-decades-1980s)**
* **[1990s Movies](https://mdblist.com/lists/ryankeast/movies-decades-1990s)**
* **[Best of the 1990s](https://mdblist.com/lists/rjchignell/best-of-the-1990-s)**
* **[2000s Movies](https://mdblist.com/lists/ryankeast/movies-decades-2000s)**
* **[2010s Movies](https://mdblist.com/lists/ryankeast/movies-decades-2010s)**
* **[2020s Movies](https://mdblist.com/lists/ryankeast/movies-decades-2020s-a2h6mk0dh0)**
* **[Christmas Movies](https://mdblist.com/lists/hdlists/christmas-movies)**
* **[Thanksgiving Movies](https://mdblist.com/lists/hdlists/thanksgiving-movies)**
* **[Best Halloween Movies of All Time](https://mdblist.com/lists/hdlists/halloween-movies-the-best-of-all-time)**
* **[Top Valentine's Movies](https://mdblist.com/lists/craigywulse23/top-valentines-movies)**
* **[St. Patrick's Day](https://letterboxd.com/blood_countess/list/st-patricks-day/)**
* **[Day of the Dead: Mexican Horror](https://letterboxd.com/cinemathek_zlb/list/dia-de-los-muertos-mexican-horror-the-full/)**
* **[Movies Based on True Stories](https://mdblist.com/lists/slander2328/movies-based-on-a-true-story)**
* **[Superhero & Comic Book Movies](https://mdblist.com/lists/jmla/superhero-based-on-comic-superhuman-abilities)**
* **[Movies Based on Video Games](https://mdblist.com/lists/awesomeaustn/movies-based-on-video-games-live-action)**
* **[Movies Based on Books](https://mdblist.com/lists/godzgiftmm/based-on-a-book-uncollected)**
* **[Biographies](https://letterboxd.com/nislav2001/list/biographies/)**
* **[60 Minutes or Less](https://mdblist.com/lists/roolfer/higesht-rated-unwatched-60-minutes-or-less)**
* **[90 Minutes or Less](https://mdblist.com/lists/roolfer/highest-rated-unwatched-90-minutes-or-less)**
* **[Under 2 Hours](https://mdblist.com/lists/stephenwall95/popular-movies-under-2-hours)**
* **[Long Movies](https://letterboxd.com/frantz/list/long-movies/)**
* **Trakt Most Favorited - Weekly**

### 📺 Series Lists
* **-Trakt Watchlist**
* **Series Recommended for you**
* **[New Streaming Releases: Series](https://mdblist.com/lists/garycrawfordgc/latest-tv-shows)**
* **[Trending Series on Trakt](https://mdblist.com/lists/snoak/trakt-s-trending-shows)**
* **[IMDb Top 250 Series](https://trakt.tv/lists/2143363)**
* **[Comedy Series](https://mdblist.com/lists/garycrawfordgc/comedy-shows)**
* **[Popular Thriller Series](https://mdblist.com/lists/snoak/thriller-shows)**
* **[Horror Series](https://mdblist.com/lists/garycrawfordgc/horror-shows)**
* **[Fantasy Series](https://mdblist.com/lists/MaxtronTV/fantasy-tv-shows)**
* **[Popular Romance Series](https://mdblist.com/lists/snoak/popular-romance-shows)**
* **[New Romance Series](https://mdblist.com/lists/snoak/latest-romance-shows)**
* **[Popular Animation Series](https://mdblist.com/lists/snoak/animationanime-shows)**
* **[Adult Animation](https://mdblist.com/lists/breon64/adult-animation)**
* **[Warner Bros. Television Studios - Series](https://mdblist.com/lists/jstinchcombe8642/warner-bros-television-studios-series)**
* **[Universal Television - Series](https://mdblist.com/lists/jstinchcombe8642/universal-television-series)**
* **[Sony Pictures Television - Series](https://mdblist.com/lists/jstinchcombe8642/sony-pictures-television-series)**
* **[20th Television - Series](https://mdblist.com/lists/jstinchcombe8642/20th-television-series)**
* **[Paramount Television Studios - Series](https://mdblist.com/lists/jstinchcombe8642/paramount-television-studios-series)**
* **[CBS Studios - Series](https://mdblist.com/lists/jstinchcombe8642/cbs-studios-series)**
* **[Lionsgate Television - Series](https://mdblist.com/lists/jstinchcombe8642/lionsgate-television-series)**
* **[MGM Television - Series](https://mdblist.com/lists/jstinchcombe8642/mgm-television-series)**
* **[ABC Signature - Series](https://mdblist.com/lists/jstinchcombe8642/abc-signature-series)**
* **[FX Productions - Series](https://mdblist.com/lists/jstinchcombe8642/fx-productions-series)**
* **[NBCUniversal Content Studios - Series](https://mdblist.com/lists/jstinchcombe8642/nbcuniversal-content-studios-series)**
* **[Bad Robot Production](https://mdblist.com/lists/jstinchcombe8642/sony-pictures-television-studios-series)**
* **[Fremantle North America - Series](https://mdblist.com/lists/jstinchcombe8642/fremantle-north-america-series)**
* **[Skydance Television - Series](https://mdblist.com/lists/jstinchcombe8642/skydance-television-series)**
* **[A+E Studios - Series](https://mdblist.com/lists/jstinchcombe8642/ae-studios-series)**
* **[Argentinian Series](https://mdblist.com/lists/mxtrakttv/argentina-series)**
* **[Best Korean Series](https://mdblist.com/lists/saltydude/top-rated-korean-tv-shows)**
* **[Spanish Series](https://mdblist.com/lists/ftor327/spain-series)**
* **[Popular Spanish Series](https://mdblist.com/lists/snafuki/spain-popular-tv-shows)**
* **[Japanese Series](https://mdblist.com/lists/nuguns17/japanese-shows)**
* **[UK Series](https://mdblist.com/lists/garycrawfordgc/channel-4-shows)**
* **[Brazilian Series](https://mdblist.com/lists/gussouzanow/brazilian-shows)**
* **[Indian Series](https://mdblist.com/lists/cakepopcorn/top-rated-indian-shows)**
---

## 🤝 Credits & Acknowledgments

- A massive shoutout to the creator of [SEL-Filtering-and-Sorting](https://github.com/Tam-Taro/SEL-Filtering-and-Sorting) for the underlying sorting rules and filtering framework.
- The open-source developers behind the AIOStreams and AIOMetadata projects for creating these powerful addon engines.
