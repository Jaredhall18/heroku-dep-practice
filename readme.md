Steps for creating a new project. Start with your mkdir {filename}
touch index.js //Makes a new file for you

create a gitignore file using npx
    npx gitignore node
    //build me a gitignore file suitable for node projects

git init

create package.json
    npm init -y

Within Plock. Create a start script.
    "start": "node index.js"

install some additional dependencies
    express
    dotenv

Now you can set up your index.js to get a server running.
Create a .env file (this is gitignored!)
//we can set a test port # for our environment here

Go to Github and create a new repo.

To add the project, use the following command script
git remote add origin git@github.com:Jaredhall18/heroku-dep-practice.git


