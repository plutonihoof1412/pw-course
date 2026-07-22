
## Git Locations
- **WorkingDir**: personal playground, can add code locally
- **Staging Area**: temporary holding place for all changes before committing
- **Local Repository**: place for the committed changes locally
- **Remote Repository**: GitHub server for sharing & backing up code

## Git Commands
### run once for a new folder (of a new project)
- `git init`: to initialize a local repo or re-initialize an existing one
- `git remote add origin ‹url›`: to create GitHub repo & connect it to the local repo
### run every time changes are made
- `git status`: to check the current location of the file
- `git log`: to check the commit history
- `git add .` or `git add {{file name}}`: to push file(s) from local to Staging, ready for finalization
- `git commit -m "feat: message"`: to push the file(s) from Staging to the local repo (finalize snapshot of the staged changes)
- `git push origin main`: to send the files to the remote repo
  
### Author identity unknown
#### tell Git who we are for all repo
- git config --global user.email "uyen@gmail.com"
- git config --global user.name "Uyen"
#### tell Git who we are for a specific repo
> must run the command inside terminal for that repo
- git config user.email "uyen@gmail.com"
- git config user.name "Uyen"

### Convention for commit commands
> **< type > : < 50-word description >**
- `chore`: small changes, typo fix, file removal
- `feat`: to add new functionality, new test case
- `fix`: to fix a test case error
