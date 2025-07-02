# [Basalt SRS](https://basalt-website.vercel.app/)

A Spaced Repetition System (SRS) application designed to work with Obsidian vaults. Basalt SRS helps you memorize important information from your Obsidian notes using AI-generated flashcards and spaced repetition.

---

## Disclaimer

**Basalt SRS is most useful for people who take notes and organize them in folders in [Obsidian](https://obsidian.md/).** However, it can be used by anyone with an Obsidian vault structure. The app is designed to leverage your existing folder and note organization for optimal spaced repetition and card generation.

---

## Features

- Add cards to specific files in obsidian
- Card Generation:
  - Manually
  - Using indentation rules
  - AI Powered (Gemini)
- Support for media attachments within cards
- Spaced repetition learning (SRS) to review cards
- Multiple review modes: Normal SRS and Cram Mode
- Card browsing and search
- Auto-update support via GitHub Releases

---

## Getting Started

### 1. Organize Your Vault
- For best results, organize your notes in folders within your Obsidian vault.
- Add YAML frontmatter tags to your notes:
  - Use `#qa` for question/answer style notes with the top-level bullet points as questions, and nested sub-level bullet points as the answer.
  - Use `#mem` for notes you want to use AI to generate cards for.

### 2. Install Basalt SRS

#### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Google AI Studio API key (for card generation), that you can get here at (Google AI Studio)[https://aistudio.google.com/app/apikey]

#### Installation
- For most users go to releases and download the appropriate .dmg file, mount the dmg, and drag Basalt SRS into Applications.

### 3. Bypass Unidentified Developer on macOS
When opening the .dmg for the first time, macOS may prevent the app from launching due to it being from an "unidentified developer."

To open the app anyway:
1. Try opening the .app file—macOS will likely block it.
2. Go to System Settings > Privacy & Security.
3. Scroll down to the Security section. You’ll see a message that says something like:
4. “Basalt SRS was blocked from use because it is not from an identified developer.”
5. Click "Open Anyway".
6. A new popup will appear. Click "Open" again to confirm.

Basalt SRS will now launch, and you won’t have to do this again for future launches.

This is a standard macOS security feature for all apps not notarized through Apple's paid developer program. There’s no risk in running Basalt SRS if you downloaded it from the official source.


### 4. First Steps in the App
1. **Select your Obsidian vault** and the folder you have storing all images in your obsidian vault. 
2. The app will scan your vault and and you should see it in the dashboard.
3. I reccomend using the in-file Q&A method FIRST to generate any cards you can. THe cards from this method will be exact and accurate.
4. THEN use the AI card generation to generate cards from any files that don't have this top-level bullet question indented sub-level bullet answer format (see below for what that means)
5. You're gonna have a bunch of new cards after you do this, so just stay on top of it and get going.



---

## Card Creation Methods


1. **Manual Card Creation**
   - Open the manual card creation window to write your own Q&A cards.
2. **QA Indented Bullets Card Extraction**
   - Extracts Q&A pairs from notes tagged with `#qa`.
   - The format used is as follows:
   - ____________ <- Question here top level bullet
     - ___________ <- Answer here in the sub bullet
   - Basalt will generate cards from all bullets in the file that have this format.
3. **AI Card Generation**
   - Uses Google AI to generate flashcards from your notes.
   - Select files/folders, specify number of cards per file (would suggest starting with 5-10 cards per file), click "Generate Cards (AI)".

---

## Reviewing Cards

- **Normal Review (SRS):**
  - Review cards due for spaced repetition.
  - Progress is tracked and cards are scheduled for optimal retention.
- **Cram Mode:**
  - Review all cards in a folder or selection, regardless of SRS schedule.
  - Great for last-minute studying.

---

## Browsing Cards
- Use the card browser to search, filter, and view all cards in your vault.
- Edit or delete cards as needed.

---

## Auto-Update
- Basalt SRS supports auto-updates via GitHub Releases.
- When a new version is released, you'll be notified in-app and can update with one click—no need to manually download or reinstall.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

## License

This project is licensed under the MIT License - see the LICENSE file for details. 
