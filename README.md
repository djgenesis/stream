---

# "Stream app" Setup and Configuration

This repository contains a fully optimized collection of ready made and maintained by this repo configuration templates and formatting files for **AIOStreams**, **Collections**, and **CustomFusionBadges**.

This guide provides the easiest path to streaming on a TV using Android and Windows devices. Everything is synced automatically inside the streaming app across all your devices.

---
<img width="2048" height="1152" alt="quick_dial_backdrop" src="https://github.com/user-attachments/assets/b6be40b5-9fc9-4bd2-9902-49ceb0dd0dbf" />
<img width="137" height="82" alt="all_popular_movies_logo" src="https://github.com/user-attachments/assets/02624673-8776-4166-a7ed-8a612bef4438" />
<img width="128" height="101" alt="best_popular_movies_logo" src="https://github.com/user-attachments/assets/a3e05a2d-0621-4184-a443-cb65c3b5a38a" />
<img width="130" height="104" alt="completed_tv_series_logo" src="https://github.com/user-attachments/assets/dc2d471f-2813-4292-9ed0-d573311f5dfd" />
<img width="188" height="87" alt="christmas_movies_logo" src="https://github.com/user-attachments/assets/f71a0afb-8ae1-406d-ba4e-1204fd818fd1" />
<img width="199" height="111" alt="new_popular_movies_logo" src="https://github.com/user-attachments/assets/1e114e39-4138-49a0-b416-91f734298671" />
<img width="2424" height="1080" alt="Screenshot_20260908-151520" src="https://github.com/user-attachments/assets/266f2412-0ea7-4bed-b3b4-81c294a21713" />
<img width="367" height="1290" alt="Screenshot_20260908-151727" src="https://github.com/user-attachments/assets/ad632e89-c575-4125-ab59-00dc5839288a" />
<img width="540" height="2877" alt="Screenshot_20260908-151843" src="https://github.com/user-attachments/assets/45313ecb-1494-48f0-81d7-f60294b1d032" />



## 📋 Prerequisites & Things You Need

### Devices Required

1. **For Watching (TV):** An Android TV, Google TV, or Android TV Box connected to your TV.
2. **For Setup:** An Android phone/tablet or a Windows PC.

### Accounts & API Keys

Before starting, ensure you have set up the following accounts:

1. **An active Debrid Subscription** (e.g., RealDebrid, AllDebrid, Premiumize, etc.).
2. **Accounts and API Keys** for metadata and layout providers (you will input these keys during configuration):

* [`Trakt.tv`](https://trakt.tv/)

3. **Addon Instance Uptime Status:** Select active addon instances and monitor their real-time status at [IbbyLabs Uptime](https://www.google.com/search?q=https://uptime.ibbylabs.dev/).

⚠️ **Important Infrastructure Advice:** For optimal performance and system stability, use **only one instance for AIOStreams** (or a single secondary instance strictly as a backup).

---

## 🚀 Complete Step-by-Step Setup Guide

### Step 1: Prepare Your TV / TV Box

1. Turn on your TV or Android TV Box.
2. Open the **Google Play Store** and install the **streaming app**.
3. Open the app on your TV. It will display a **QR Code** and a **Web URL Link**.
4. **Leave this screen open on your TV.** *(We do this first to confirm your TV operating system supports the application before configuring addons)*.

---

### Step 2: Set Up the App on Your Setup Device (Phone or PC)

1. On your Android phone/tablet (via Google Play Store) or Windows PC (via official website), open the streaming app.
2. **Sign Up** using your email and log in to your account.

---

### Step 3: Retrieve Your Debrid API Key

1. Open a web browser, go to your chosen Debrid service (RealDebrid, AllDebrid, Premiumize, etc.), and log in.
2. Navigate to **Account Settings**.
3. Copy your **API Key**. Keep this browser tab open as you may need it later.

---

### Step 4: Configure AIOStreams

1. Open the configuration page for an active **AIOStreams** instance (check [IbbyLabs Uptime](https://www.google.com/search?q=https://uptime.ibbylabs.dev/)).
2. Click **Upload / Import Template** and select `aiostreams-config.json` or `aiostreams-template.json` from this repository.
3. Paste your **Debrid API Key** under your debrid service section.
4. Choose your preferred formatting route:

* **Route A (Recommended - Custom Badges):** Load `formatter-usingbadges.json`.
* **Route B (Plain Text):** In Formatter settings, click Save and load `formatter-notusingbadges.json`.

5. Click **Install / Generate Link**. This will automatically prompt to open the Addon in the streaming app.
6. Click **Install** inside the streaming app.

---

### Step 5: Configure Collections (Recommended for Optimum Experience)

1. Add [Quick Dial](https://nuvio.tv/community-collections/quick-dial) to your profile (created and maintained by this repo).
2. Add [ImKaptain Mega Collection](https://nuvio.tv/community-collections/kaptain-s-mega-collection-v0-4) to your profile.
3. If you have other profiles repeat steps 1 and 2 by switching to each profile first.
4. Every so often (Once a month or even twice a year) Import to each profile the file QuickDial&ImKaptainCombo.json to keep your collections up to date.

---

### Step 6: Player & Subtitle Settings (Recommended for Optimum Experience)

1. In the streaming app, go to **Settings — Streams**.
2. Paste the raw URL of `gold_badges_complete.json` [https://raw.githubusercontent.com/djgenesis/stream/refs/heads/main/gold_badges_complete.json](https://raw.githubusercontent.com/djgenesis/stream/refs/heads/main/gold_badges_complete.json) (created and maintained by this repo) into **Fusion Badges URLs**. Disable size badges and addon logo, and set the badge position to **Top**.
3. Go to **Settings — Advanced** and select **Remember last profile**.
4. Click the **Settings (Gear Icon)** on the left sidebar:

* Select your preferred **Interface Language**.
* Set your **Default Subtitles Language**.
* Enable **Autoplay next episode** (recommended for TV series).

---

### Step 7: Watchlist Sync & Tracking (Recommended for Optimum Experience)

1. Create a free account at [trakt.tv](https://trakt.tv/) if you don't have one.
2. Inside the app, go to **Settings → Tracking** and connect your Trakt account to back up your watch history and sync watchlists.

---

### Step 8: Link Your Account to Your TV

1. Go back to your TV screen where the QR code and link are displayed.
2. **If using an Android Phone/Tablet:** Scan the QR code on the TV screen using your phone camera/scanner.
3. **If using a Windows PC:** Open a browser, visit the web link shown on the TV, and log in with your credentials if requested.
4. Your TV / TV Box will automatically authorize and enter the app interface!
5. Go to **Settings — Advanced** and select **Remember Last Profile**.

---

### Step 9: Test Your Setup

1. Go to the **Discover** section on your TV app.
2. Click on any Movie or TV show.
3. Select a stream from the results list.
4. The video should start playing within 2 to 5 seconds depending on file size and internet connection.

*And voilà! WE ARE DONE!*

---

## 👥 Family / Extra Member Login Process

Follow these steps when setting up an extra device or family member profile:

### Things Required

* An Android TV, Google TV, or Android TV Box connected to the TV.
* An Android phone/tablet or Windows PC.
* An active account with [`Trakt.tv`](https://trakt.tv/)
* The original primary member's account credentials OR another active profile member to grant you access.

### Steps

1. **On TV / TV Box:** Install the streaming app from the Google Play Store. Open it so the QR code and login link are displayed.
2. **On Phone / PC:** Open the streaming app website or mobile app and log in using the **original primary member's account credentials**.
3. **Sync TV:** Scan the QR code with your phone or enter the web link on your PC browser.
4. Your TV / TV Box will automatically log into the account.
5. **Profile Customization:**

* Go to **Settings — Advanced** and enable **Remember last profile**.
* Go to **Settings → Tracking** and connect an individual Trakt.tv account if personal watch history tracking is desired.

6. **Test:** Head to **Discover**, select a stream, and start watching!

---

## 📌 Important Notes & FAQ

* **VPN Requirement:** You **do NOT need a VPN** to stream content using this setup. Your ISP will not flag or throttle your connection because streams are delivered via secure web servers (HTTPS direct streaming) rather than peer-to-peer torrents.
* **Cross-Device Syncing:** Everything you configure (adding/removing addons, organizing watchlists, updating settings) automatically syncs across every device logged into your account.

Happy streaming! 🎬

---

## 📁 Included Movie & Series Catalogs (frequently updated)

By importing `media-collections.json`, the following dynamic catalogs will be automatically integrated into your library interface:
"djb" lists are maintained by... yours truly.
Here is the complete summary of all movie and TV lists provided in the file, including item counts where available:

---

### **General & Trending**

* **Popular Movies (djb)**: This dynamically updated MDBList filter set aggregates roughly 60 popular, featured, and trending lists across platforms like Trakt, TMDb, IMDb, Rotten Tomatoes, major streaming services, top user collections, and movie leaks. To ensure high-quality content, it targets English-language titles released within the last 365 days that meet strict baseline metrics: an IMDb rating over 6.0 with at least 1,000 votes, and an overall MDBList score of 40 or higher.


* **New Popular Movies (djb)**: This list is updated on a weekly basis and includes ONLY the NEW additions that occur every week from the list * **Popular Movies (djb)**


* **Completed TV Series / Documentaries (djb)**: 100 items. This list features completed TV series with a minimum rating of 60/100, organized so that the shows wrapping up most recently appear first.


* **Christmas Movies (djb)**: 1,000 items. Updated daily throughout the Christmas season (every year during November and December), this collection aggregates holiday movies compiled from over 60 top user lists. It applies targeted filters to feature English-language, released titles that meet a base threshold of an IMDb rating above 5.0 with at least 10 votes.


* **Movies Recommended for You**: Trakt List


* **Series Recommended for You**: Trakt List


* **New Streaming Releases: Movies**: 200 items


* **New Streaming Releases: Series**: 300 items


* **Latest 4K Movies**: 111 items


* **In Cinemas Now**: 5 items


* **Trending Movies on Trakt**: 235 items


* **Trending Series on Trakt**: 250 items


* **Top Movies of the Month**: 15 items


* **IMDb Top 250 Series**: Trakt List


* **Top 100 Classic Movies**: Trakt List



---

### **Action & Superheroes**

* **Top Action Movies**: 541 items


* **New Action Releases**: 500 items


* **Modern Action**: 140 items


* **1980s Action**: Trakt List


* **Action Movies (2000 - 2020)**: Trakt List


* **Top 10 Action Movies Of 21st Century**: Trakt List


* **Action Comedy**: Trakt List


* **Kung Fu Action**: Trakt List


* **Superheroes**: Trakt List



---

### **Comedy & Stand-Up**

* **Top Comedy Movies**: 4,153 items


* **Comedy Series**: 300 items


* **New Releases in Comedy**: 500 items


* **Stand-ups**: 773 items


* **Top 100 TV Comedy Shows**: Trakt List


* **British Comedy**: Trakt List


* **20 Minute Comedy**: Trakt List


* **Australian Comedy**: Trakt List



---

### **Thriller & Mystery**

* **Popular Thriller Movies**: 500 items


* **Popular Thriller Series**: 500 items


* **New Thriller Releases**: 500 items


* **Psychological Thriller**: 99 items


* **Espionage Thrillers**: Trakt List


* **IMDb's Top Thriller Movies**: Trakt List


* **50 Best Indian Psychological Thriller Films**: Trakt List


* **Political Thrillers**: Trakt List


* **Korean Mystery Thrillers**: Trakt List


* **Investigative Thrillers**: Trakt List



---

### **Horror**

* **Top Horror Movies**: 903 items


* **New Horror Releases**: 500 items


* **Horror Series**: 140 items


* **Rotten Tomatoes: Best Horror Movies Of All Time**: Trakt List


* **The Horror Club: The Best Of Slasher Flicks**: Trakt List


* **Hidden Horror Gems**: Trakt List


* **French Horror**: Trakt List


* **Asian Horror**: Trakt List


* **Japanese Horror**: Trakt List


* **Classic Horror**: Trakt List


* **Comedy Horror**: Trakt List



---

### **Sci-Fi & Fantasy**

* **Top Fantasy/Sci-Fi Movies**: 900 items


* **Fantasy Series**: 232 items


* **Best Fantasy Comedy**: Trakt List


* **Classic Sci-Fi & Fantasy**: Trakt List


* **Fantasy: Swords, Sorcery, and Celluloid**: Trakt List


* **Dark Fantasy Collection**: Trakt List



---

### **Romance**

* **Popular Romance Movies**: 500 items


* **Popular Romance Series**: 200 items


* **New Romance Series**: 200 items


* **Best of Romance**: 500 items


* **Romantic Comedies**: Trakt List


* **Teen Romance**: Trakt List


* **Wartime Romance**: Trakt List


* **Romance, Fantasy & Comedy Crossovers**: Trakt List


* **Forbidden Love in Movies**: Trakt List


* **IMDb's Top Romance Movies**: Trakt List



---

### **Animation & Franchise Collections**

* **Popular Animation Movies**: 500 items


* **Popular Animation Series**: 500 items


* **Adult Animation**: 207 items


* **Pixar Animation Studios**: Trakt List


* **Dreamworks Animation**: Trakt List


* **Sony Pictures Animation**: Trakt List


* **Hidden Animation Gems**: Trakt List


* **IMDb's Top Animation Movies**: Trakt List


* **Warner Bros Animation**: Trakt List


* **Japanese Anime Movies**: Trakt List


* **Fox Adult Animation**: Trakt List


* **Garfield Collection**: Trakt List


* **Scooby-Doo Collection**: Trakt List


* **Shrek Collection**: 20 items



---

### **Documentaries & Musicals**

* **Music Concerts & Documentaries**: Trakt List


* **Music Documentaries**: Trakt List


* **Live Concerts & Music**: Trakt List


* **True Crime Documentaries**: Trakt List


* **Attenborough Documentaries**: Trakt List


* **Rotten Tomatoes: Best Documentaries**: Trakt List


* **History Documentaries**: Trakt List


* **BBC Wildlife & Nature Documentaries**: Trakt List


* **Hacking & Programming Documentaries**: Trakt List


* **Space Documentaries**: Trakt List


* **War Documentaries**: Trakt List


* **AFI Greatest Movie Musicals**: Trakt List


* **Live Stage Musicals**: Trakt List



---

### **Actor Collections**

* **Robert De Niro**: 216 items


* **Al Pacino**: 119 items


* **Meryl Streep**: Trakt List


* **Jack Nicholson**: Trakt List


* **Anthony Hopkins**: 155 items


* **Morgan Freeman**: 186 items


* **Daniel Day-Lewis**: 25 items
---

## 🤝 Credits & Acknowledgments

* Shoutout to the creator of [SEL-Filtering-and-Sorting](https://github.com/Tam-Taro/SEL-Filtering-and-Sorting) for the underlying sorting rules and filtering framework.
* The open-source developers behind the AIOStreams and AIOMetadata projects.
