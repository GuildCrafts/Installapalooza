# Installfest Step 1.1: Node.js & Express Stack

Most of the coding work we do at Learners Guild will be driven by the back-end web development framework [Express](http://expressjs.com). We'll install Express individually in each project we create. For now, we'll install the other tools we'll use along with Express.

#### Plan Overview

1. Install Node.js, a platform for back-end web development with the JavaScript programming language.
1. Install PostgreSQL, the database we'll use with our Node.js and Express stack.

## Node.js

__Note:  when copying the code snippets, please exclude the `$` as you paste and run the code into your terminal.  The dollar sign `$` is simply an indicator of the logged-in user's terminal prompt in the examples.__

1. Install Node.js with Homebrew by running the following command in the Terminal:

  ```bash
  $ brew install node
  ```

2. Run the Terminal command `node -v` to check that Node.js was installed. It should print a version number greater than or equal to "v5.8.0". The Terminal command `node` changes your Terminal into a Javascript REPL ("Read Evaluate Print Loop"), like the right-hand side of repl.it. Use the shortcut `ctrl + c`, or type `.exit` to quit out of the REPL and return to the normal Terminal prompt.

2. Run the Terminal command `which npm` to check that NPM is installed. The Node Package Manager, used through various `npm` commands, is a lot like Homebrew, except we'll use it for Node.js-specific tools instead of for general Mac tools. NPM packages are often called "node modules."

### Nodemon

Nodemon (short for "node monitor") will make our Node.js workflow more efficient.

1. Install nodemon globally with the following Terminal command:

  ```bash
  $  npm install -g nodemon
  ```

## PostgreSQL  

### Postgres

1. Install postgres via Homebrew
  ```bash
  $ brew install postgres
  ```

2. Configure postgres to start when the system does.

  ```bash
  $ mkdir -p ~/Library/LaunchAgents

  $ ln -sfv /usr/local/opt/postgresql/*.plist ~/Library/LaunchAgents
  ```


3. Check that your install worked

    ```bash
    $ which psql
    ```

    If it worked, you should see ```/usr/local/bin/psql``` as the terminal output.

## Next Up
* [x] Set up your Node.js environment
* [ ] Install Development Tools
