# Good-Night
Sleep is something everyone does - but not everyone does well.

We noticed that many of our own peers struggle with falling asleep. Sometimes it is academic stress. Sometimes it is personal anxiety. Sometimes it is deeper- past trauma, repeated nightmares, or chronic overthinking that refuses to quiet down at night.

We began looking into research papers on insomnia and sleep difficulty. Across multiple studies, we saw common causes repeatedly cited:

Hyperarousal and stress activation
Anxiety and depressive symptoms
Behavioral loops (irregular sleep schedules, excessive screen exposure)
Conditioned wakefulness (“bed = awake”)
Sensory overstimulation

One insight stood out clearly:
There is no single cause of sleep difficulty - and therefore no single solution.

Yet when we looked at existing apps, most of them focused on one or two aspects only:
music apps, meditation apps, therapy apps, reminder apps, tracking apps.

We asked ourselves:
What if there was one platform that addressed all dimensions of sleep?
That is how Good Night was born.

##What We Learned
Through research and prototyping, we learned that sleep is a multidimensional system.
If we define sleep readiness as a function:
𝑆=𝑓(𝐵,𝐸,𝑆𝑒,𝐻,𝐶)
Where:
B = Behavioral regulation
E = Emotional support
Se = Sensory environment
H = Health integration
C = Community accountability

Most existing apps optimize for only one variable.
Nightlight was designed to optimize for all five.

We learned that:
Behavioral tools alone are insufficient without emotional grounding.
Sensory tools (white noise, music) work differently for different people.
Community accountability increases routine adherence.
Health reminders influence long-term sleep consistency.
Privacy is foundational when dealing with sleep and mental health data.

Sleep is personal. There is no universal template.

##Our Solution
Good Night is a one-stop sleep ecosystem integrating:

*Behavioral Regulation*
Digital Sunset to dim screens and reduce distraction
Structured wind-down timer
Personalized sleep goals (fall asleep faster, reduce nightmares, etc.)
Mood tracking and AI-adjusted sleep targets

*Emotional Support*
AI chatbot for late-night thoughts
Journal & dream rewriting tools
Direct therapist contact integration

*Sensory Tools*
White, brown, and pink noise
Ambient music and lullabies
Curated Sleepy TV visuals
Voice reader and audiobook support

*Physical Relaxation*
4-4-6 guided breathing exercises
Snuggle Stretch (yoga-based calming routines)
Calming stretch mode for immediate drift-off support

*Health Integration*
Medication tracking
Appointment reminders
Health data synchronization
Emergency contact setup

*Community Accountability*
Support groups (Nightmare Survivors, 8-Hour Club, Zen Masters)
Peer discussions
Safe community space with confidentiality protections

And to make the experience warmer, we added Luma, an interactive digital companion that grows with user consistency and adds emotional engagement to an otherwise clinical space.

##How We Built It
This project pushed us technically in ways we had not experienced before.

*Design*
Designed entirely in Figma
Used Figma Make to iterate rapidly on UI flow
Focused on calming color systems and soft visual hierarchy

*Frontend*
Built using React Native
Type-safe component architecture
Custom UI styling with CSS
Modular layout for ritual, library, and health components

*Backend & APIs*
Used 11 Labs API for Luma voice/chat integration
Connected via .json structured API calls
Built database integration for health reminders and medication tracking
Managed context-based state systems for rewards and ritual tracking

##Challenges We Faced
This project was technically ambitious — and that meant real obstacles.

*API Looping Issues*
During early AI implementation, responses were returning in repetitive static loops.
We had to retrain prompts, restructure API calls, and provide richer contextual data to ensure dynamic, meaningful outputs.

*Feature Regression During Iteration*
As we iterated and personalized features, some components were lost in newer versions.
We had to carefully manage state handling and modular architecture to prevent data loss.

*Privacy & Data Security*
Because sleep and mental health data are sensitive, privacy was non-negotiable.

We designed the system to:
Store data locally by default
Require explicit permission for syncing
Separate API handling from health database layers
Maintaining this architecture added complexity — but it was essential.

Removed Sleep Graph Feature
We initially implemented a sleep log graph visualization.
However, UI rendering conflicts caused stability issues during live updates.
Rather than compromise stability, we chose to remove it for this version.

If we had more time, we would:
Rebuild the graph component using a more stable charting library
Integrate longitudinal sleep pattern analytics

##What This Project Means to Us
Good Night is more than an app.

It represents:
The understanding that sleep struggles are common
The belief that no one should navigate anxiety alone at night
The idea that technology can feel warm, not cold
The responsibility to treat user data with care
We built Nightlight not as a feature list, but as a system.

Sleep is complex.
People are complex.

Our solution respects that complexity.
