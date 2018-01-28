#Bloc Identity
##Set up guide
### Install node js (to get npm)
- go to https://nodejs.org/en/ (for windows install)
- for mc install homebrew:
open a terminal and type
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
then install npm 
in a terminal type
brew install node
- once installed in a terminal type
node -v 
you should get back the node version installed 

### Install node red
- for windows in a command prompt type
npm install -g --unsafe-perm node-red
- for mac, in a terminal type
sudo npm install -g --unsafe-perm node-red


### Start node red
In  a terminal/ command prompt type
node-red
This should start the service

In a browser go to:
http://localhost:1880
You should see node red running

###Import the project
Go to menu > Import > clipboard
Paste in the contents of blocIdentity.json

###Get the bloc chain nodes
Go to menu > Manage Palette > search 'blocchain'
Add the 'node-red-contrib-blockchain' nodes

###Add local files
Find where node-red is installed (will be in <your home>/.node-red/ )
Edit settings.js 
Find and uncomment httpStatic, change to a folder you want to have your node-red images in e.g.
httpStatic: '<full path to your home>/.node-red/images/',
Paste eyescanner.png into this folder (in /images)
Restart node-red (in the terminal ctrl C and then 'node-red')

##Start the app
Go to node-red http://localhost:1880
Click deploy
Go to http://localhost:1880/blocIdentityform







