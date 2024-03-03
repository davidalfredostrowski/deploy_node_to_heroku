https://forum.freecodecamp.org/t/building-a-node-js-application-using-docker/463269
https://stackoverflow.com/questions/26595874/heroku-src-refspec-master-does-not-match-any
https://help.heroku.com/LGKL6LTN/how-do-i-delete-destroy-a-heroku-application
https://stackoverflow.com/questions/45001168/npm-err-missing-script-start-error-with-docker
https://www.docker.com/blog/getting-started-with-docker-using-node-jspart-i/
https://stackoverflow.com/questions/15693192/heroku-node-js-error-web-process-failed-to-bind-to-port-within-60-seconds-of

ls
sudo apt-get update
sudo apt-get install -y ca-certificates curl gnupg
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/nodesource.gpg
NODE_MAJOR=20
echo "deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_$NODE_MAJOR.x nodistro main" | sudo tee /etc/apt/sources.list.d/nodesource.list
sudo apt-get update
sudo apt-get install nodejs -y
node -v
sudo snap install docker
npm install express --save
curl https://cli-assets.heroku.com/install-ubuntu.sh | sh
sudo npm install -g heroku --force
heroku --version
heroku login -i
mkdir alfredo
cd alfredo/
vi Dockerfile
vi app.js
vi heroku.yml
vi package.json
cd ..
ls
npm install express --save
vi .dockerignore
cd alfredo
ls
sudo docker build -t alfredo .
sudo docker run -p 8080:8080 -tid alfredo
heroku create alfredoone --manifest

git init
git add -A
git commit -m "firstfirst"
git branch -M main
heroku git:remote -a alfredoone
git push heroku HEAD:master
