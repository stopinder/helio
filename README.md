[README_Heliosynthesis.md](https://github.com/user-attachments/files/20544468/README_Heliosynthesis.md)

# Heliosynthesis – Reflective Supervision & Journaling App

Heliosynthesis is a desktop-first Vue 3 application designed for therapists and clients to engage in reflective journaling, parts mapping, and symbolic self-exploration. Built using a clean modular architecture with Supabase as backend and Whisper for optional voice input.

---

## 🚀 Project Setup

```bash
git clone https://github.com/yourusername/heliosynthesis.git
cd heliosynthesis
npm install
npm run dev
```

Make sure to configure your `.env` file with Supabase keys.

---

## 🧱 Project Structure

```
/src
  /components        → Reusable UI components
  /views             → Main pages: Chat, Journal, Map, etc.
  /store             → Pinia store for global state
  /assets            → Images, icons, and CSS
```

---

## 🗺️ Core Screens

- `ReflectiveChat.vue`: AI journaling interface
- `NewJournalEntry.vue`: Structured prompt entry
- `SystemMap.vue`: Visual graph of IFS parts and relationships
- `SymbolicModal.vue`: Slide-in drawer for archetype selection
- `Clients.vue`: Therapist-facing dashboard for client list
- `Settings.vue`: Mode toggles, theme preferences

---

## 🔐 Supabase Notes

- **Auth:** Email login (JWT)
- **Tables:** `users`, `journal_entries`, `parts`, `clients`
- **Storage:** Optional image uploads and symbolic assets

---

## 🎙️ Whisper Voice Input (Planned)

- Microphone access via browser
- Audio sent to OpenAI Whisper API
- Transcript returned to populate journal entry input

---

## 🧩 System Map Tech

- Visualization TBD (e.g., Vue Force Graph or D3)
- Nodes support labels, part types, and relationships:
  - `Protects`, `Fears`, `Suppresses`, `Supports`

---

## 🛠 Dev Notes

- Vue 3 + Vite
- Tailwind CSS for styling
- Pinia for state management
- Supabase SDK v2
- Deployed on Vercel (optional: Docker config in `/docker` folder)

---

## 👤 Author

Developed by Robert Ormiston  
Psychotherapist (IFS & EMDR-informed)  
Website: [robormiston.com](https://robormiston.com)

---

## 📄 License

MIT (or update this as needed)

