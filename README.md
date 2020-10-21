# How to get started with Ethereum blockchain development

## Using Truffle Suite and React

## Prerequisites:
* Node
* Understanding of React framework
* Terminal of choice

## How to begin
1. Install truffle. We're going to install truffle globally, using npm. Enter into your terminal:

    `npm install -g truffle`

1. Make a directory for your new project and navigate to your new directory:

    `mkdir truffle-example`

    `cd truffle-example`

1. Unbox a truffle box. We're going to use one called drizzle. There are many other boxes available too:

    `truffle unbox drizzle`

1. Let's see what we have. Open the contents in your text editor of choice. For example, I'm using vs-code `code` command:

    `code .`


    ## (Brief explanation on what we have inside our unboxed drizzle project)

1. Open a new terminal window and navigate into our React app:

    `cd app`

1. Start the react app running locally on your computer:

    `npm start`

    you should see a loading... message because there is no blockchain to connect to. Let's get one running locally on our computer using [ganache-cli](https://www.npmjs.com/package/ganache-cli)

1. Open a new terminal window. We're going to install ganache-cli globally:

    `npm install -g ganache-cli`

1. Run ganache-cli to get a local ethereum blockchain running on your computer. 

    `ganache-cli`

    when successful, this command will provide you with 10 available accounts and corresponding private keys, each account with 100 ETH. Will also provide a mneumonic or 12-word phrase. The blockchain will listen on port 8545

1. Create a command to run our blockchain as deterministic and mnemonic:

    in our code editor, we are going to edit our package.json inside our truffle-example directory. We are going to create a command called `ganache-cli` to run our blockchain and persist it to a db.

    
  ``
