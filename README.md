# AdvancedNodeStarter

You need to log in or sign in into Google developers' console and do as follows:

1. Enable Google+ API

2. Set up OAuth consent screen https://console.developers.google.com/apis/credentials/consent

3. Create credentials https://console.developers.google.com/apis/credentials (Oauth Client Id) and copy them for later use

3a. Authorize JavaScript origins with:

http://localhost:5000

3b. Authorized redirect URIs:

http://localhost:5000

http://localhost:3000/auth/google/callback

4. Save and wait a few minutes so everything propagates over the network.

Afterward, update config/dev.js file with the new credentials along with the mongoAtlas DB string you created in mongoAtlas.

In addition, I had to update the package.json on the server the following dependencies:

"mongoose": "^5.6.7",

"passport": "^0.4.0",

"passport-google-oauth20": "^2.0.0",

Make sure you delete the package-lock.json before running npm install again.

Once you have done the above-mentioned changes, the project should work as planned.

Cheers!
