# ACME http file server

Super simple express fileserver as needed for ACME challenge to obtain Let's Encrypt certificate, with the folder structure already in place.

Usage:

1. `git clone` this repo
2. change the filename and content under `.well-known/acme-challenge` to the strings given by the ACME client (e.g. certbot)
3. `node server.js`
4. check browser if file is served
