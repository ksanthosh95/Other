# 💍 Shanthosh & Vishruthaa — Wedding Digital Invitations 🌹

A responsive, culturally authentic, and royal Tamil Chettiyar wedding web invitation suite crafted for **Shanthosh & Vishruthaa**, celebrating their wedding ceremonies on **November 14th & 15th, 2026** at **AVS Mahal, Sathyamangalam, Erode District, Tamil Nadu**.

This project is optimized for static hosting on **GitHub Pages**, providing interactive celebration details, calendar sync, commute concierges, and traditional wedding music.

---

## 🌟 Available Invitation Themes

| File | Theme | Description |
| :--- | :--- | :--- |
| **[`marriage-invitation.html`](./marriage-invitation.html)** | 🍷 **Royal Chettiyar Maroon & Gold** | Traditional Athangudi palace crimson, gold foil gradients, deepam oil lamps, and warm royal wedding aesthetics. |
| **[`marriage-invitation-blue.html`](./marriage-invitation-blue.html)** | 🌌 **Royal Midnight Sapphire & Gold** | Regal midnight dark blue & sapphire gradients paired with lustrous radiant gold foil borders and dual-tone petals. |
| **[`engagement-invitation.html`](./engagement-invitation.html)** | 🌸 **Engagement Ceremony Card** | Elegant digital invitation card for the auspicious engagement celebration. |

---

## ✨ Interactive Features

- 🎵 **Background Wedding Music**: Ambient audio player playing *"Maalai Saarthinaal"* with animated sound-wave indicator and floating toggle button.
- 🌸 **Petal Shower Canvas**: Real-time particle animation scattering gold, champagne, and floral petals across the screen.
- ⏳ **Dual-Event Live Countdown**: Dynamic countdown switcher for both:
  - **Grand Reception**: Friday, Nov 14, 2026 @ 7:00 PM
  - **Subha Muhurtham**: Saturday, Nov 15, 2026 @ 9:00 AM – 10:30 AM
- 📅 **Add to Calendar**: Instant calendar integration for Google Calendar, Outlook Calendar, and one-click `.ics` file downloads for Apple Calendar.
- 📍 **Interactive Venue & Navigation**: Full address, Google Maps direct route links, and one-tap venue address clipboard copying.
- 🚆 **Outstation Commute Guide**: Interactive tabbed guide for guests traveling from:
  - **Bengaluru (~220 km)**: Vande Bharat / Intercity Express train guides, road routes via NH44, and direct sleeper bus operators (Silk Board, Madiwala, Marathahalli).
  - **Chennai (~420 km)**: Vande Bharat Express (20643) schedules, overnight Cheran/Nilgiri Express, and flights via Coimbatore (CJB).
- 🏞️ **Regional Sightseeing Concierge**: Nearby heritage and nature spots for outstation family and friends (Bannari Amman Temple, Kodiveri Dam, Bhavani Sagar Dam).
- 📱 **Mobile & WhatsApp Optimized**: Fully responsive layout with Open Graph meta tags for rich social sharing cards on WhatsApp.

---

## 📂 Repository Structure

```text
Wed-invite/
├── marriage-invitation.html        # Main Wedding Invitation (Royal Maroon & Gold)
├── marriage-invitation-blue.html   # Main Wedding Invitation (Royal Midnight Blue & Gold)
├── engagement-invitation.html      # Engagement Invitation Card
├── Malaai_saarthinaal.mp3         # Traditional wedding nadaswaram audio
├── Keethan_-_Kalale...cut.mp3      # Alternate celebration music track
├── chettiyar-wedding-bg.jpg        # Traditional Chettiyar palace architecture backdrop
├── chettiyar-wedding-bg2.jpg       # Alternate atmospheric background texture
└── README.md                       # Project documentation & deployment guide
```

---

## 🚀 How to Host on GitHub Pages

1. **Initialize Git Repository** (if not already done):
   ```bash
   cd /path/to/Wed-invite
   git init
   git add .
   git commit -m "Initial commit of wedding invitations"
   ```

2. **Push to your GitHub Repository**:
   ```bash
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git branch -M main
   git push -u origin main
   ```

3. **Set Default Landing Page**:
   - To make one of the invitations open automatically at `https://<your-username>.github.io/<repo-name>/`, duplicate or rename your preferred theme to `index.html`:
     ```bash
     # To use the Royal Maroon theme as default:
     cp marriage-invitation.html index.html

     # OR to use the Royal Dark Blue theme as default:
     cp marriage-invitation-blue.html index.html
     ```

4. **Enable GitHub Pages**:
   - In your GitHub repository, go to **Settings** > **Pages** (in the left sidebar).
   - Under **Build and deployment** > **Branch**, select `main` and `/ (root)`, then click **Save**.
   - Within 1–2 minutes, your wedding invitation will be live at:
     ```text
     https://<your-username>.github.io/<repo-name>/
     ```

---

## 🛠️ Customization Guide

### 1. Changing the Background Music
In both `marriage-invitation.html` and `marriage-invitation-blue.html`, locate the `<audio>` tag around line 1730:
```html
<audio id="bgWeddingAudio" loop preload="auto">
    <source src="Malaai_saarthinaal.mp3" type="audio/mpeg">
    <source src="https://raw.githubusercontent.com/<your-username>/<repo>/main/Malaai_saarthinaal.mp3" type="audio/mpeg">
</audio>
```
You can replace the local file path or CDN link with your preferred audio file.

### 2. Updating Venue / Event Timings
- Event dates and countdown targets can be updated in the JavaScript `switchCountdown` function:
  ```javascript
  currentCountdownTarget = new Date('November 14, 2026 19:00:00 GMT+0530').getTime();
  ```
- Calendar links can be updated directly in the Google Calendar URL parameters.

---

## 📜 Credits & Warm Blessings

- **Couple**: Shanthosh & Vishruthaa
- **Ceremony Date**: November 14 & 15, 2026
- **Venue**: AVS Mahal, Sathyamangalam, Tamil Nadu
- *"A celebration of new beginnings, a promise of forever, and the joy of sharing it with our dearest ones."*
