Lepton 3.5 viewer

Install the 'qt4-dev-tools' package, which allows compiling of QT applications.
- sudo apt-get install qt4-dev-tools

To build (will build any SDK dependencies as well):
- cd viewer
- qmake && make

To clean:
- make sdkclean && make distclean

Install imagemagick to convert png to jpg:
- sudo apt-get install imagemagick


Set password to os environment:
- sudo apt-get install vim
- vim ~/.bashrc
- add following to the end of file: export SERVER_PASSWORD="password from skype"
- esc + :wq
- source ~/.bashrc

To start download image to server:
- sudo apt-get install build-essential libssl-dev libffi-dev python3-dev
- cd .. (you should be at project root directory now (lepton_raspberry_pi/)
- pip3 install -r requirements.txt

To start everything:
- cd viewer (from where you are)
- ./start_script.sh & (image saving)
- cd ../ssh_scripts
- python3 app.py & (send images to server)

Know your mac address (bag here):
- cd ..
- python3 mac_address.py

(!NOTE: better to use screen daemon instead of &) 
(- sudo apt-get install screen)
