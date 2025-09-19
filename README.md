# Smriti AI – Your Smart Learning Companion

Smriti AI is an intelligent, all-in-one learning assistant that helps you **organize**, **understand**, and **retain** everything you study 🧠. Whether you're a student, a self-learner, or a professional, Smriti AI transforms passive content into active learning tools.

## 🛠️ Tech Stack

- 🧩 **Frontend**: Next.js, TypeScript, Tailwind CSS
- 🧠 **AI Layer**: Gemini APIS,LLMs
- 🔐 **Auth**: Clerk
- ☁️ **Backend**: Next.js,Prisma,Postgres
- 🤖 **Bot Layer**: WhatsApp + Twilio Integration
- 🧪 **Chrome Extension**: Capture videos directly from YouTube //upcoming
## 📸 Screenshots

Here’s a quick look at **Smriti AI in action** 👇

<p align="center"><b>🏠 Homepage</b></p>
<p align="center">
  <img src="./screenshots/Home.jpg" alt="Homepage" width="80%"/>
</p>

<p align="center"><b>🚀 Getting Started</b></p>
<p align="center">
  <img src="./screenshots/GettingStarted.jpg" alt="About" width="80%"/>
</p>

<p align="center"><b>📊 Dashboard</b></p>
<p align="center">
  <img src="./screenshots/Dashboard.jpg" width="80%"/>
</p>

<p align="center"><b>⏰ Study Reminder</b></p>
<p align="center">
  <img src="./screenshots/StudyReminders.jpg" width="80%"/>
</p>

<p align="center"><b>📝 Topic-wise Notes</b></p>
<p align="center">
  <img src="./screenshots/TopicWisenotes.jpg" width="80%"/>
</p>





![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 🚀 Getting Started (Developer Mode)

Follow these steps to set up Smriti AI locally:

### 1. Set Up Supabase (Database)

1. Go to [https://supabase.com](https://supabase.com)
2. Create a new project
3. Copy the connection string and add it to your `.env.local` file:

```ini
DATABASE_URL=your_supabase_connection_string
```

### 2. Run Database Migrations

```bash
npx prisma generate
npx prisma db push
npx prisma studio # optional, for DB UI
```

### 3. Get API Keys & Configure Environment

#### Clerk (Authentication)

- Go to [https://dashboard.clerk.com](https://dashboard.clerk.com)
- Create a new application
- Add the following to `.env.local`:

```ini
CLERK_PUBLISHABLE_KEY=your_key
CLERK_SECRET_KEY=your_key
```

#### Google Gemini (AI)

- Go to [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)
- Add to `.env.local`:

```ini
GEMINI_API_KEY=your_key
```

#### YouTube API (Optional)

- Go to [https://console.cloud.google.com](https://console.cloud.google.com)
- Enable YouTube Data API v3
- Add to `.env.local`:

```ini
YOUTUBE_API_KEY=your_key
```

#### Cloudinary (Optional, for media uploads)

- Go to [https://cloudinary.com](https://cloudinary.com)
- Add to `.env.local`:

```ini
CLOUDINARY_CLOUD_NAME=your_name
CLOUDINARY_API_KEY=your_key
CLOUDINARY_API_SECRET=your_secret
```

#### Twilio (WhatsApp Reminders)

- Go to [https://www.twilio.com/console](https://www.twilio.com/console)
- Create a new project and get your credentials
- Add the following to `.env.local`:

```ini
TWILIO_ACCOUNT_SID=your_account_sid
TWILIO_AUTH_TOKEN=your_auth_token
TWILIO_PHONE_NUMBER=whatsapp:+14155238886 # Example format for WhatsApp
```

#### RapidAPI (YouTube Video Summarization)

- Go to [YouTube Video Summarizer GPT AI on RapidAPI](https://rapidapi.com/rahilkhan224/api/youtube-video-summarizer-gpt-ai/playground)
- Subscribe and get your API credentials
- Add the following to `.env.local`:

```ini
RAPIDAPI_HOST=your_rapidapi_host
RAPIDAPI_KEY=your_rapidapi_key
RAPIDAPI_URL=your_rapidapi_url
```

### 4. Install Dependencies & Run the App

```bash
git clone https://github.com/vatsal-bhakodia/smriti-ai
cd smriti-ai
npm install
npm run dev
```

The app should now be running at [http://localhost:3000](http://localhost:3000) 🚀
