# simon-game-ci-walkthrough
On terminal when you want to initiate the project open terminal and write:

- npm init
- package name: keep the name or you can change it  (press Enter)
- version: (press Enter)
- Entry point: index.js (press Enter)
- test command: jest   (IMPORTANT TO ENTER THIS VALUE AND PRESS ENTER TO SET THE TESTER AS JEST)
- git repository: the url of the repo
- keywords: (press Enter)
- author: (press Enter)
- licens: (press Enter)
- Is this OK ? (press Enter)

now you can install jest also on termianl write below: you want to install jest as a development dependency
- npm install jest --save-dev

to check if it's work after install it and try it write on terminal:
- npm test




///*******************************************
## With this project we learned:
- principles of software testing (basic software testing)
- principles of test-driven development
- how to test DOM and DOM events
- how to expose the inner working of a function for testing
- how to build a small of dobust project using tests



always below code to use for every html document:

beforeAll(() => {
    let fs = require("fs");
    let fileContents = fs.readFileSync("index.html", "utf-8");
    document.open();
    document.write(fileContents);
    document.close();
})
