# Bundle 1 - Exercise 1

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git init
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "resolving conflict file"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git remote add origin https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git pull origin main --allow-unrelated-histories
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "committing change"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b div
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch -m div dev
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin -u dev
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b test
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout dev
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch -d test
# Bundle 1 - Exercise 2

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash push -m "incomplete about.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash push -m "incompelete team.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash push -m "incomplete home.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash pop "stash@{2}"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash pop "stash@{0}"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "new file changed"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash pop "stash@{0}"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "last file "
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin dev
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash push -m "new change on team.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash pop "stash@{0}"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git reset --hard
# Bundle 2 - Exercise 1

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/bundle-2
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\services.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "file: services.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/bundle-2
# Bundle 2 - Exercise 2

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add index.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "file for all information"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/service-redesign
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\services.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat : new line added"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin  ft/service-redesign
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add services.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "looking conflict and resolving it"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout ft/service-redesign
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git merge main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\services.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "resolved merge conflict with main"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin ft/service-redesign
# Bundle 3 - Exercise 1

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/team-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add team.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat: changes on team.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/team-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/contact-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout ft/team-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\README.md
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m ""