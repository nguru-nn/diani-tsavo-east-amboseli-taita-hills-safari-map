

Readme · MD
# Diani Beach → Tsavo East, Amboseli & Taita Hills: 4-Day Safari Route Map
 
An interactive 3D map of a 4-day road safari from **Diani Beach** on Kenya's south coast. The trip begins with a game drive across **Tsavo East**, continues to **Amboseli** beneath Kilimanjaro, and ends with a night at the famous stilted **Salt Lick Safari Lodge** in the **Taita Hills Wildlife Sanctuary**.
 
🗺️ **See the full itinerary and the live map:**
[Cztery dni zwiedzania: Tsavo Wschód, Amboseli i Taita Hills](https://safarikenia.com.pl/cztery-dni-zwiedzania-tsavo-wschod-amboseli-taita-hills/) on **Safari Kenia**
 
---
 
## The route
 
| Stop | Park | Accommodation |
|------|------|---------------|
| Start | Diani Beach | — |
| Day 1 | Tsavo East National Park | Voi Safari Lodge |
| Day 2 | Amboseli National Park | Amboseli Sopa Lodge |
| Day 3 | Taita Hills Wildlife Sanctuary | Salt Lick Safari Lodge |
| Day 4 | Return to Diani Beach | — |
 
**Day 1:** Diani Beach → Likoni Ferry → Buchuma (Bachuma) Gate. From the gate, a game drive runs through the heart of Tsavo East to Voi Safari Lodge.
**Days 2–3:** Voi → Amboseli → Taita Hills.
**Day 4:** Taita Hills → Mariakani → Likoni Ferry → Diani Beach.
 
The interface labels are in Polish, matching the tour page it's embedded on.
 
## Features
 
- **Game drive traced inside the park.** Waypoints inside Tsavo East make the route follow the in-park tracks from Buchuma Gate to Voi, instead of the main highway.
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain at 1.5× exaggeration, plus a tilted camera. This makes the Taita Hills rise sharply out of the Tsavo plains.
- **Road-accurate route.** Each leg comes from the Mapbox Directions API (driving profile) and is stitched into one line. If a request fails, the map falls back to a straight segment for that leg.
- **Animated route line.** A golden "marching ants" dashed line runs over a soft glow layer.
- **Interactive itinerary panel.** A glassmorphism sidebar lists each day. Clicking a card flies the camera to that lodge and opens its popup.
- **Custom markers.** Gold SVG pins mark each overnight stop. Hidden waypoints shape the route without cluttering the map.
- **Mobile-friendly.** On small screens the sidebar becomes a bottom sheet, and cooperative gestures keep page scrolling smooth.
- **WordPress-ready.** Styles are scoped to one container, so the code can be pasted into a Custom HTML block.
## Tech stack
 
- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, no build step
- Plus Jakarta Sans (Google Fonts)
## Usage
 
1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own, and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.
To change the route, edit the `itineraryData` array. Entries with `isWaypoint: true` shape the route only. All other entries get a marker and a sidebar card.
 
## About
 
Built for [Safari Kenia](https://safarikenia.com.pl/), Polish-language safari tours and travel guides for Kenya.
 
➡️ [View this 4-day safari itinerary](https://safarikenia.com.pl/cztery-dni-zwiedzania-tsavo-wschod-amboseli-taita-hills/)
 
