# URLShortener - Cloud-based URL Shortener SaaS

<img src="https://github.com/user-attachments/assets/13b97230-20a6-4cd2-b0b2-5ac4b9afb43d" width="30%">

Inspired by [https://codingchallenges.fyi/challenges/challenge-url-shortener/](https://codingchallenges.fyi/challenges/challenge-url-shortener/)

## Features
- **SHA-256 Hashing**: Hash urls with high Preimage Resistance
- **Collision proofing**: Use an iterative string approach to ensure Second Preimage Resistance 
- **Speeedup**: Retrieve <k,v> pairs lightning fast using Redis data store


## Components

The system consists of two main components:
1. **Node Server (`app.js`)**: A Node js server that creates a socket server to intake a longURL and store the <longURL,shortURL> pair in Redis  
2. **Frontend Gui (`vite-project/src/App.tsx`)**: A Tailwind-designed frontend that defines GET and POST API requests through Express routing

## Installation
git clone using https or SSL
For the purpose of local Redis, you will need to download Redis using Bash/zsh/WSL

## Usage
1. In the .env folder in the root directory, change the `LINEAR_STRING` value to a custom value
   
**⚠️ Do not leave blank as it opens up the possibility to probe the original url**

2. Open two Command Prompt windows
4. Run `node app.js` to start the backend server
5. Navigate to the 'vite-project' folder and run `npm run dev` to start the Gui

## Technologies
<div align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=express,githubactions,js,nodejs,react,redis,tailwind,vercel" />
  </a>
</div>

## Disclaimer

The author makes no guarantees of the efficacy or security of this application for anything other than personal use
