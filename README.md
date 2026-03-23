# Chatify - Real-Time Chat Application

A modern, real-time chat application built with React, Supabase, and Tailwind CSS.

## Features
- **Real-Time Messaging**: Instant message delivery using Supabase PostgreSQL subscriptions.
- **Presence & Online Status**: See who's online in real-time.
- **Typing Indicators**: Visual feedback when someone is composing a message.
- **User Profiles**: Custom usernames, bios, and avatar uploads (Supabase Storage).
- **Public Chat Rooms**: Create and join multiple chat rooms.
- **Premium UI**: Modern dark theme with glassmorphism and smooth animations.

## Tech Stack
- **Frontend**: React (Vite), Tailwind CSS, Lucide React
- **Backend**: Supabase (Auth, Database, Storage, Realtime)
- **Icons**: Lucide React

## Setup Instructions

### 1. Supabase Setup
- Create a new project on [Supabase](https://supabase.com).
- Run the `supabase_schema.sql` (found in the root) in the **SQL Editor**.
- Enable **Storage** and create two public buckets: `avatars` and `message-images`.
- Add your **Project URL** and **Anon Key** to the `.env` file.

### 2. Installation
1. Clone or download the project.
2. Open a terminal in the project directory.
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

## Development
- `src/lib/supabase.js`: Supabase client configuration.
- `src/pages/Dashboard.jsx`: Main chat logic and real-time handling.
- `src/pages/Auth.jsx`: Authentication flow and initial profile creation.
- `src/pages/Profile.jsx`: Profile management and avatar uploads.
