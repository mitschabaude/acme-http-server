# ACME http file server

Super simple express fileserver as needed for ACME challenge to obtain Let's Encrypt certificate, with the folder structure already in place.

Intended usage is after the first couple of steps of `certbot certonly --manual` or similar, with a setup where node.js can directly listen to requests from the outside.

Usage:

1. `git clone` this repo
2. change the filename and content under `.well-known/acme-challenge` to the strings given by certbot
3. `node server.js` (as root, because we listen to port 80)
4. check browser if file is served
