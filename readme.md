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

Now we can create a project on heroku to get this deployed!

Conversely:
Using heroku instead of GIT.

    Login via CLI:
        heroku login

    heroku git:remote -a {name of app on heroku!}

    git push main heroku

IF ERRORS -- check logs
    heroku logs -a <project name in  heroku> --tail


We can do a full-stack project and deploy that too!
    npx create-react-app client

add a script to plock 
    "heroku-postbuild": "cd client && npm i && npm run build"

This should create a build folder inside of client with your static assets.

We added server.use in index.js and server.get to allow the deployment to find these files and directory.
