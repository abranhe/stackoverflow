[View on StackOverflow](https://stackoverflow.com/a/52521809/7602110)

Here are the steps, in detail ...

- Install **Node.js** from [nodejs.org/en/download](https://nodejs.org/en/download/)

- Update to the latest version of **npm**:  `$ npm install npm -g`

- Make a new folder for the **npm** global packages `$ mkdir ~/.npm-packages`

- Tell **npm** where to find/store them `$ npm config set prefix ~/.npm-packages`

Verify the install


    # this should show the versions
    node -v  
    npm -v  
    # this should show npm and ng with no errors
    npm list -g --depth=0

Hope it works for you, it worked for me!
