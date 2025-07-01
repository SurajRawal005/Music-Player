# 🎵 Spotify Clone Music Player

A sleek, responsive Spotify-inspired music player built using **React**, **Tailwind CSS**, and **React Router**, with **Context API** for managing global player state.

---


## 🔗 Live Demo 

👉 [Click to Open the App](https://music-player-u5if.vercel.app/)


## 🚀 Features

- 🎧 **Play/Pause** songs
- ⏭️ **Next/Previous** track control
- 📀 **Album & Song Lists** displayed in clean UI
- 🔊 **Progress bar (seek control)**
- 🎨 **Dynamic album background gradients**
- 🧠 **Global audio control using Context API**
- 📱 **Responsive Design** (mobile/tablet/desktop)

---

## 🛠️ Tech Stack

| Tech        | Purpose                          |
|-------------|----------------------------------|
| React       | Frontend UI                     |
| React Router| Page Routing (Home, Album)      |
| Tailwind CSS| Styling                         |
| Context API | Music state & controls          |
| useRef      | Audio DOM control (seek, play)  |

---

## 📁 Folder Structure

src/
│
├── assets/ # Static assets (icons, images, data)
│
├── components/
│ ├── AlbumItem.jsx
│ ├── Display.jsx
│ ├── DisplayAlbum.jsx
│ ├── DisplayHome.jsx
│ ├── Navbar.jsx
│ ├── Player.jsx
│ ├── Sidebar.jsx
│ └── SongItem.jsx
│
├── context/
│ └── PlayerContext.jsx # Global audio logic
│
├── App.jsx
├── index.jsx
└── index.css

yaml
Copy
Edit

---

## 🧠 How State Works

- `PlayerContext.jsx` uses `useRef` to control the `<audio>` tag.
- Functions like `play()`, `pause()`, `next()`, and `previous()` update the player globally.
- Time updates and progress bar (`seekBar`) are synced via `ontimeupdate` and refs.

---

## 🧪 To Run the Project

```bash
# Clone the repo
git clone https://github.com/yourusername/spotify-clone.git

# Navigate to the folder
cd spotify-clone

# Install dependencies
npm install

# Start dev server
npm run dev
📸 Preview

💡 Future Improvements
Add search functionality 🔍

Save playlists to local storage or backend 💾

Auth integration (Login/Profile) 🔐

Backend connection for real-time music API 🎼
