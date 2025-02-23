# Project Goal: 
- Facilitate the ability for a user to search for a song using the Spotify API, that they can then vote to be played next. 

## Functional Requirements: 
- Users are directed to the page via a QR Code
- Users can see the current song playing
- Users can see the queue of songs currently being voted on. 
- Users can search for a song and add to the queue.
- Users can vote up or down a song in the queue.
- Once the current song ends, the most upvoted song is played next.

### Technical Challenges
- API will need to be secured, without the initial requirement of supporting user logins.
- Browser Fingerprinting for preventing spam voting could become a requirement depending on use cases.
  - Potential Tool: https://github.com/FoxIO-LLC/ja4/tree/main
- A decision will need to be made on how long to retain songs in the queue, as well as for how long a session will last (length of song, timed duration, until EOD, etc)

## System Design & Architecture 
- Pending

## Technology Choices & Rationale
### UI & UX - NextUI
https://www.heroui.com/

Rationale: As this is a new-build with no predefined brand identity to follow or established Design Language, a simplified UI kit will be enough for initial development while mitigating the need for extensive styling. 

### Front-End - Next.js
https://nextjs.org/

Rationale: Though the page can be built using plain HTML, CSS, & Javascript, this presents an opportunity to explore modern front-end frameworks. 
This can be pivoted to later on, but due to the componetized nature of features it may be more prudent to use a framework to begin with. 

### Back-end & API - Python & Flask
https://vercel.com/templates/next.js/nextjs-flask-starter
https://flask.palletsprojects.com/en/stable/

Python was selected to continue to build on the experience Chris has with Python. Flask handles the API endpoints that the front end will utilize. 

### Hosting Partner
- Pending
