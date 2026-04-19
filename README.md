# IPTV Playlist (Updated)

Last verified: 2026-04-18

---

## বাংলা

### সমস্যা কেন হচ্ছিল
- বেশিরভাগ স্ট্রিম লিংক মেয়াদোত্তীর্ণ ছিল
- অনেক লিংক private/internal IP (`172.x.x.x`) ব্যবহার করছিল, যা পাবলিক নেটওয়ার্কে কাজ করে না
- কিছু সোর্স ডোমেইন বন্ধ/অকার্যকর ছিল

### আপডেট করা হয়েছে
- `running.m3u` → যাচাইকৃত, চলমান বাংলা চ্যানেল লিংক দিয়ে আপডেট
- `play.m3u` → `running.m3u`-এর একই আপডেটেড কাজের লিংক
- `world.m3u` → যাচাইকৃত আন্তর্জাতিক + বাংলা মিশ্র কাজের লিংক
- `ipl.m3u` → আপডেটেড স্পোর্টস স্ট্রিম লিংক
- `channels/*.m3u8` থেকে প্রাসঙ্গিক কয়েকটি ফাইলে নতুন working source বসানো হয়েছে

### প্লেলিস্ট লিংক
- Bangla (Primary): `https://lupael.github.io/IPTV/running.m3u`
- Bangla (Mirror): `https://lupael.github.io/IPTV/play.m3u`
- World: `https://lupael.github.io/IPTV/world.m3u`
- Sports / IPL: `https://lupael.github.io/IPTV/ipl.m3u`

### ব্যবহার
1. VLC/Kodi/Televizo/IPTV Smarters খুলুন
2. `Open Network Stream` বা `Add Playlist URL` নির্বাচন করুন
3. উপরের যেকোনো playlist URL পেস্ট করুন

### নোট
- IPTV লিংক সময়ের সাথে পরিবর্তিত হতে পারে
- কোনো চ্যানেল বন্ধ পাওয়া গেলে Issue/PR দিন

---

## English

### Why playback was failing
- Most stream URLs were expired/outdated
- Many links pointed to private/internal IPs (`172.x.x.x`) that are unreachable from public networks
- Several source domains were offline or no longer serving valid HLS playlists

### What was updated
- `running.m3u` → refreshed with verified working Bangla streams
- `play.m3u` → synchronized with the same verified working Bangla streams
- `world.m3u` → refreshed with verified mixed global + Bangla streams
- `ipl.m3u` → refreshed with currently working sports streams
- Matching files in `channels/*.m3u8` were updated where verified replacements were available

### Playlist URLs
- Bangla (Primary): `https://lupael.github.io/IPTV/running.m3u`
- Bangla (Mirror): `https://lupael.github.io/IPTV/play.m3u`
- World: `https://lupael.github.io/IPTV/world.m3u`
- Sports / IPL: `https://lupael.github.io/IPTV/ipl.m3u`

### How to use
1. Open VLC/Kodi/Televizo/IPTV Smarters
2. Choose `Open Network Stream` or `Add Playlist URL`
3. Paste one of the playlist URLs above

### Notes
- IPTV links can change or expire over time
- If any channel goes down, open an Issue/PR with updated working source

---

## Source and validation
- Replacement links were collected from actively maintained public IPTV sources and re-checked via HTTP/HLS response validation during this update.
