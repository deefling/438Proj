Kelly - to set up, make sure you install up-to-date versions of node/npm (npm is node package manager, should install w/node)
Both should be on your path

'node -v' should be near v18.12.1
'npm -v' should be near 8.19.2

All - to set up:

run 'npm i' and it should automatically download /node_modules.

The way I am doing this is adding npm dependencies, gitignoring them & recording them in package.json
this way package.json gives npm instructions to download & update dependencies locally, rather than us uploading manually.

1 way to import dependencies in js files:
const { MongoClient } = require('mongodb');

You should be able to run npm -i anytime someone adds a new dependency and things should update on your end

'npm run start' will run index.js
'npm run dev' will use nodemon to run index.js & re-run every time you hit save
you can make more scripts like this in package.json