# anki-minerva
To get started quickly, download the [.apkg](https://github.com/amdecker/anki-minerva/releases/tag/hcs). 

## Why/How
- Official App: https://apps.ankiweb.net/. Free for desktop and Android 
### Really good readings on SRS (spaced repetition systems)
- Simple intro https://ncase.me/remember/
- Advanced intro with lots of good use cases (eg learning Unix commands, incrementally reading a complex paper, etc) http://augmentingcognition.com/ltm.html
- Another explanation with many examples of how to write good Anki cards https://andymatuschak.org/prompts/
>I believe **the most important thing to “optimize” in spaced repetition practice is the emotional connection to your review sessions and their contents**. It’s worth learning how to create prompts which effectively represent many different kinds of understanding…If you find yourself reviewing something you don’t care about anymore, you should act. Sometimes upon reflection you’ll remember why you cared about the idea in the first place, and you can revise the prompt to cue that motivation. But most of the time the correct way to revise such prompts is to **delete** them.
- Essential reading for writing good cards: https://www.supermemo.com/en/blog/twenty-rules-of-formulating-knowledge
- If you aren't already convinced to use anki https://gwern.net/spaced-repetition 
- Specific tips for language learning: a book called Fluent Forever by Gabriel Wyner (2014)
- Specific tips for math: https://cognitivemedium.com/srs-mathematics
- Reminder that these premade decks are just the start. The goal is to give you a baseline that you can make your own cards from. **Making your own cards is the best way to learn**.
- Read the docs if you want to learn more. Gives lots of good info on differences between decks and tags (use decks for material that you might want to study in isolation from other material and use tags to organize your notes), how one note can have multiple cards, etc. https://docs.ankiweb.net/

### Recommend setup
- You can backup and sync your cards across devices by making an ankiweb account 
keep all your cards and decks under on big master deck (Default) because then you will be forced to review cards from different topics next to each other which helps you learn
- Change the deck to use the FSRS scheduler instead of the default one
- Otherwise there's probably no need to change any settings 

## Editing these shared decks & integration with git
0. Ask @amdecker or subit pull request
1. Open a terminal on your computer. Make sure Anki is closed. 
2. Install [ki](https://langfield.github.io/ki/), which is a tool that integrates Anki with git. Follow the instructions for setting up ki up to and including the step ["Running the clone command"](https://langfield.github.io/ki/#running-the-clone-command). This will move your Anki decks into a local git repository in a format that ki can work with.
3. Navigate inside the ki repo: `cd collections`. Then run `git submodule add https://github.com/amdecker/anki-minerva.git` to get the shared decks. 
4. Open Anki and add cards or make changes to the cards. When you are done, close Anki. Then run `ki pull` to move the changes into the ki repo. Run `git commit -am "your commit message"` followed by `git push` to push the local changes to Github. 
