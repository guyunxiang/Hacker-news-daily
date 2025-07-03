# Show HN: Talkie Spendy – voice-first expense tracker

**Posted by talkiespendy on 2025-07-02**

Hi HN — I’m Emerik, the creator of *Talkie Spendy*, a mobile app that logs expenses through voice instead of typing. I’ve often abandoned budgeting tools because manual entry feels like homework, so I built something that records a purchase in under five seconds.

**How it works:**  
Tap once, then say “4 dollars 50 coffee at Starbucks.” The audio is sent to the ElevenLabs speech-to-text API for transcription, followed by a lightweight OpenAI prompt that extracts the amount, merchant, and category. Only this JSON data (including the original timezone) syncs to Supabase. The entire app is built with FlutterFlow, providing instant charts and CSV export features.

**Technology stack:**  
- FlutterFlow  
- Supabase Postgres + Edge Functions  
- ElevenLabs Speech-to-Text (cloud API)  
- OpenAI Language Model

**Looking for feedback:**  
I’d love your thoughts on the overall user experience—what’s confusing, what’s missing, or what could improve retention. Any ideas on making voice budgeting truly useful are very welcome.

Thanks for checking it out!