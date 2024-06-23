# anki-minerva

## Editing these shared decks
1. Open a terminal on your computer. Make sure Anki is closed. 
2. Install [ki](https://langfield.github.io/ki/), the tool integrates Anki with git. Follow the instructions for setting up ki up to and including the step ["Running the clone command"](https://langfield.github.io/ki/#running-the-clone-command). This will move your Anki decks into a local git repository in a format that ki can work with.
3. Navigate inside the ki repo: `cd collections`. Then run `git submodule add https://github.com/amdecker/anki-minerva.git` to get the shared decks. 
4. Open Anki and add cards or make changes to the cards. When you are done, close Anki. Then run `ki pull` to move the changes into the ki repo. Run `git add .` and `git commit -m "your commit message"` followed by `git push` to push the local changes to Github. 
