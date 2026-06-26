# Stremio / Nuvio Configuration Templates

This repository contains a fully optimized collection of configuration templates and formatting files for the **AIOStreams** and **AIOMetadata** addons within the Stremio / Nuvio ecosystem. It is designed to deliver premium quality stream results with rich metadata, offering two distinct visual setups (with or without custom badges).

Filtering and sorting logic is natively based on [Tam-Taro's SEL-Filtering-and-Sorting](https://github.com/Tam-Taro/SEL-Filtering-and-Sorting).

---

## 📋 Prerequisites

Before starting the setup process, ensure you have the following:
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

⚠️ **Important Infrastructure Advice:** For optimal performance and system stability, it is highly recommended to use **only one instance for AIOMetadata** and **one instance for AIOStreams** (or a single secondary instance strictly as a backup). You should select your addon instances and track their real-time uptime status here: [IbbyLabs Uptime](https://uptime.ibbylabs.dev/).

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

You can choose between **two different paths** depending on your visual preference for your stream layout:

### 🔹 Route A: Using Badges (Recommended Visual Setup)
This path provides a rich graphical experience using clean icons and gold badges for stream resolutions, formats, and audio attributes.
1. Open the configuration page of your chosen **AIOStreams** instance (pick a high-uptime instance from [IbbyLabs Uptime](https://uptime.ibbylabs.dev/)).
2. Import/Upload the [`aiostreams-config.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-config.json) or [`aiostreams-template.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-template.json) file.
3. Save and generate your installation link and add it to Stremio / Nuvio.
4. Copy the raw url of [`gold_badges_complete.json`](https://raw.githubusercontent.com/djgenesis/stream/refs/heads/main/gold_badges_complete.json) and paste it into the **Custom Badges** field of the addon configuration.

### 🔹 Route B: Not Using Badges (Text Only Setup)
This path provides a classic, distraction-free text format for users who prefer standard text strings over graphical badges.
1. Open the configuration page of your chosen **AIOStreams** instance.
2. Import/Upload the [`aiostreams-config.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-config.json) or [`aiostreams-template.json`](https://github.com/djgenesis/stream/blob/main/aiostreams-template.json) file.
3. In the **Formatter** settings, replace the contents (copy and paste the contents of [`formatter-title-notusingbadges.json`](https://github.com/djgenesis/stream/blob/main/formatter-title-notusingbadges.json) into the Title section, and [`formatter-description-notusingbadges.json`](https://github.com/djgenesis/stream/blob/main/formatter-description-notusingbadges.json) into the Description section).
4. Save and generate your installation link and add it to Stremio / Nuvio.

### 🎬 Configuring AIOMetadata
Regardless of the stream route chosen above, you must configure your metadata catalogs:
1. Open the configuration page for your chosen **AIOMetadata** instance.
2. Upload/Import the [`aiometadata-config.json`](https://github.com/djgenesis/stream/blob/main/aiometadata-config.json) file.
3. Fill out all your personalized API keys (`gemini`, `tmdb`, etc.) in their respective setup fields.
4. Save and generate the installation link and add it to Stremio / Nuvio.

---

## 📁 Included Movie & Series Catalogs

By importing the [`aiometadata-config.json`](https://github.com/djgenesis/stream/blob/main/aiometadata-config.json) profile, the following dynamic metadata catalogs will be automatically integrated into your Stremio / Nuvio library interface:

### 🎬 Movies Lists
* **Popular Movies** – Currently trending movies globally.
* **Trending Movies** – Movies experiencing a sharp spike in active views.
* **Oscar Winners & Nominees** – Curated collections of Academy Award historical winners and current nominees.
* **Box Office Hits** – Top-grossing recent theatrical releases.
* **Top Rated (IMDb/TMDB)** – All-time fan-favorite and critically-acclaimed films.
* **New Releases** – Newly available digital releases, VODs, and theatrical titles.
* **Sci-Fi & Fantasy Essentials** – Handpicked essential cinema masterworks within the Sci-Fi and Fantasy genres.

### 📺 Series Lists
* **Popular TV Shows** – The most-watched television series worldwide.
* **Trending Series** – Television shows generating the highest social engagement and viewership metrics right now.
* **Top Rated Shows** – Highest-rated television productions based on community reviews.
* **Highly Anticipated / Returning Shows** – Highly awaited new seasons and brand new series releases.
* **Anime Seasonal Catalogs** – Dedicated anime discoverability broken down by current broadcasting seasons.
* **Streaming Platform Originals** – Consolidated networks catalogs showcasing premium original productions (Netflix, HBO, Disney+, Apple TV+, etc.).

---

## 🤝 Credits & Acknowledgments

- A massive shoutout to the creator of [SEL-Filtering-and-Sorting](https://github.com/Tam-Taro/SEL-Filtering-and-Sorting) for the underlying sorting rules and filtering framework.
- The open-source developers behind the AIOStreams and AIOMetadata projects for creating these powerful addon engines.
