# MyTaskList - Mean App From Scratch
This repository is based on the Traversy Media youtube tutorial with the same title.

The directory structure as shown in the tutorial follows an old Angular.io quickstart approach
that is no longer published on the Angular.io website.

The website now directs readers to employ a quickstart approach that uses a Quickstart seed repository found
on github at https://github.com/angular/quickstart.  Unfortunately, this approach is somewhat different from the youtube
tutorial and most of us Angular 2 newbies are unable to continue with the tutorial.

This repository solves the problem by incorporating the Quickstart seed into the tutorial.  You can continue
following along with the youtube tutorial if you follow these steps:
  1.  You can clone this repository in its entirety and use it to continue with the tutorial.  Alternatively, you can
      continue using your project files and simply clone the Quickstart seed repo mentioned above inside  your 'client'
      project folder.  
  2.  If you read the Quickstart seed Readme file, you will be instructed to remove numerous unnecessary files.  This
      repository has already removed those files.
  3.  You will note in this repository that the index file from the Quickstart seed has been moved from 
      'client/src/index.html' to replace the index.html file at 'client/views/index.html.'  If you decided not to clone
      this repository you will also need to move the file and make a couple of changes to it.  The path references on two
      scripts must be changed by adding 'src' to the beginning of the path string.  The index.html file in this repo has
      already been edited to reflect the correct paths.
  4.  The 'systemjs.config.js' file in this repo has also been edited at about the 14th line.  It was changed from
      " app: 'app', "  to  " app: 'src/app' "  Make sure your 'systemjs.config.js' file reflects this change.
  5.  At this point everyone should cd into the 'client' folder from his/her terminal.  Run 'npm install' to download and
      install the angular node modules.  A node_module folder will be created inside the 'client' directory.  If you cloned
      this repository and are missing the node_modules folder in the root directory you will also need to run 'npm install'
      from the root directory to re-install the server modules.  At this point you should have two node_modules folders in
      your project.  One in the root (topmost) directory of your project and another in the 'client' directory.
  6.  After this you need to cd back into the 'client' folder.  You will then run "npm run build:watch" to
      compile the typescript (ts) files into javascript.  Running this command will also keep watch for any changes to
      your 'ts' files and recompiles them as soon as you save any changes.  NOTE: this command is not running a 'server,'
      it is merely running a typescript compiler.  Do not run the server from within this directory.
7.  Open up another terminal window.  Go back to your root directory and make sure the express server that you have been 
    previously running is shut down.  Run 'node server' or 'nodemon' from within this directory to start your application.  
    Open your browser and navigate to 'localhost:3000'  You should see "Hello Angular"see "Hello Angular"
