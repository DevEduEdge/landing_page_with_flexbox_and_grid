#Install Node.js and npm: If you don't have them already, download and install Node.js from nodejs.org. npm (Node Package Manager) comes bundled with it.

#Initialize your project: Open your project folder in VS Code's terminal and run npm init -y to create a package.json file.

#Install Browser Sync: In the terminal, run npm install browser-sync --save-dev (remove *--save-dev* for installing globally )

#Configure Browser Sync: You can either use the command line or create a bs-config.js file for more complex setups. Here's a simple example using the command line: -{ browser-sync start --server --files "**/*.html, **/*.css, **/*.js" } copy the line of code within {}

#Note - If save locally within project. 
1) open folder in terminal or bash
2) run the command - { ./node_modules/.bin/browser-sync start --server --files "**/*.html, **/*.css, **/*.js" } without {}
3) This tells the terminal to execute the browser-sync command located within the .bin folder inside node_modules.

Running via script
1) Open your package.json file > "scripts" add the below commmand, you can change the execution command {start} as well 
2) add this command -  "scripts": {"start": "browser-sync start --server --files \"**/*.html, **/*.css, **/*.js\""}
3) now run the {command you have set} from bash or terimial