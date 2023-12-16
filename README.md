Skip to content
Robystis
/
whatsapp-bot-md

Code
Pull requests
Actions
Projects
Wiki
Security
Insights
Settings
Owner avatar
whatsapp-bot-md
Public
forked from lyfe00011/whatsapp-bot-md
Robystis/whatsapp-bot-md
Add file
This branch is up to date with lyfe00011/whatsapp-bot-md:master.
Folders and files
Name		
Latest commit
lyfe00011
lyfe00011
fix tiktok
77ff43c
 · 
2 days ago
History
.github/ISSUE_TEMPLATE
Update issue templates (lyfe00011#149)
last year
lib
fix tiktok
2 days ago
media
first
last year
plugins
fix
last month
.gitignore
add wcg
9 months ago
.replit
0
last year
Dockerfile
fix
2 months ago
Procfile
logout in truecaller
2 months ago
README.md
var DISABLE_START_MESSAGE
4 months ago
app.json
logout in truecaller
2 months ago
config.js
add bing
last month
heroku.yml
fix
2 months ago
index.js
fix
2 months ago
package.json
fix tiktok
2 days ago
replit.nix
0
last year
yarn.lock
fix
2 months ago
Repository files navigation
README
WhatsApp MD User Bot
A simple WhatsApp User bot.

Setup
Deploy on Heroku

Click SCAN and scan the QR code through the "WhatsApp Linked Devices" option in your WhatsApp app.
You will get a session ID in WhatsApp, copy the ID only.
If you don't have an account on Heroku, create an account now.
If you don't have a GitHub account, sign up now.
FORK this repository.
Now DEPLOY.
Deploy on Koyeb

Create an account on Koyeb. Sign up now.
Get DATABASE_URL. You'll need this while deploying.
Get SESSION_ID. Open Linked Devices in WhatsApp and SCAN now.
Get the Koyeb API key. Let's Go.
DEPLOY now.
Enter Environment Variables. Read More.
Enter a name and click "Create Service."
Deploy on VPS or PC (Example here as in Ubuntu)

Install with script

wget -N -O levanter.sh http://bit.ly/43JqREw && chmod +x levanter.sh && ./levanter.sh
Install without a script

Install git, ffmpeg, and curl:

sudo apt -y update && sudo apt -y upgrade
sudo apt -y install git ffmpeg curl
Install nodejs:

sudo apt -y remove nodejs
curl -fsSl https://deb.nodesource.com/setup_lts.x | sudo bash - && sudo apt -y install nodejs
Install yarn:

npm install -g yarn
Install pm2:

sudo yarn global add pm2
Clone the repository and install packages:

git clone https://github.com/lyfe00011/whatsapp-bot-md botName
 cd botName
  yarn install --network-concurrency 1
Enter Environment Variables: Copy-paste the lines below (remove SESSION_ID if not needed):

echo "SESSION_ID = Session_Id_you_Got_After_Scan_Dont_Add_This_Line_If_You_Can_Scan_From_Terminal_Itself
PREFIX = .
STICKER_PACKNAME = LyFE
ALWAYS_ONLINE = false
RMBG_KEY = null
LANGUAG = en
WARN_LIMIT = 3
FORCE_LOGOUT = false
BRAINSHOP = 159501,6pq8dPiYt7PdqHz3
MAX_UPLOAD = 200
REJECT_CALL = false
SUDO = 989876543210
TZ = Asia/Kolkata
VPS = true
AUTO_STATUS_VIEW = true
SEND_READ = true
AJOIN = true
DISABLE_START_MESSAGE = false
PERSONAL_MESSAGE = null" > config.env
Read More

Edit the config.env using nano if needed. To save, press Ctrl + O, then press Enter, and to exit, press Ctrl + X.

Start and stop the bot:

To start the bot: pm2 start . --name botName --attach --time
To stop the bot: pm2 stop botName
Thanks To
Yusuf Usta for WhatsAsena
@adiwajshing for Baileys
About
A whatsapp Multi Device bot based on baileys

Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 0 watching
Forks
 15.7k forks
Releases
No releases published
Create a new release
Packages
No packages published
Publish your first package
Languages
JavaScript
99.7%
 
Other
0.3%
Suggested workflows
Based on your tech stack
Webpack logo
Webpack
Build a NodeJS project with npm and webpack.
SLSA Generic generator logo
SLSA Generic generator
Generate SLSA3 provenance for your existing release workflows
Datadog Synthetics logo
Datadog Synthetics
Run Datadog Synthetic tests within your GitHub Actions workflow
More workflows
Footer
© 2023 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact
Manage cookiesDo not share my personal informationRobystis/whatsapp-bot-md: A whatsapp Multi Device bot based on baileys
