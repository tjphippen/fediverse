# fediverse

Read:
https://sopa.tulane.edu/blog/decentralized-social-networks

## Description

The goal of this project is to provide a Dockerized Ubuntu/CentOS image that Creators can easily setup. This will automatically install & connect to multiple distributed content networks listed below, provide an Admin UI/CMS running on port 80(Like Wordpress) & serve a website/portal for public or members only content. The Creator may add plugins/modules for payments or subscriptions, themes, etc. 

All content will be stored/accessed via distributed networks. 

Admin Interface: 
  - PHP & Vue.js (running on hosted server)

Consumption Interfaces: 
  - Vue.js/CSS/HTML served from hosted server(creator's domain, theming, extended plugins)
  - Android/iOS Mobile app(TBD) (@handel for creators, official plugins supported)


## Ref

Matrix: https://matrix.org/docs/develop | https://github.com/matrix-org/dendrite

Diaspora: https://github.com/diaspora/diaspora

Mastdon: https://github.com/tootsuite/mastodon

Peertube: https://github.com/Chocobozzz/PeerTube | https://docs.joinpeertube.org/install-docker


## Creator Setup (Digital Ocean) ##

1. Goto https://cloud.digitalocean.com/droplets/new
2. Under `Choose an image` select the `Marketplace` tab, search for & select `Fediverse`??
3. Select {min-requirements} & Create Droplet!
4. Navigate to https://NEW_DROPLET_IP 
5. Login with default `user` and `password` & complete the guided setup.
