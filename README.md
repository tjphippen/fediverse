# fediverse


### Ref

Resources: https://awesomeopensource.com/project/gdamdam/awesome-decentralized-web
Element Repos: https://github.com/vector-im

## RSS 3.0
https://github.com/tartaria-nova/RSS-3.0

## Description

The goal of this project is to provide a Dockerized Ubuntu/CentOS image that Creators can easily setup. This will automatically install & connect to multiple distributed content networks listed below, provide an Admin UI/CMS running on port 80(Like Wordpress) & serve a website/portal for public or members only content. The Creator may add plugins/modules for payments or subscriptions, themes, etc. 

All content will be stored/accessed via distributed networks. 

----

## Networks
There are multiple decentralized content delivery networks. The following is a few to look into & that we may or may not end up using. Please give feedback/suggestions if there are alternatives that would better serve the goals of this project. A Node.js/npm package will be created as a wrapper to interact with the various network APIs running on the Creator's instance

Matrix: https://matrix.org/docs/develop | https://github.com/matrix-org/dendrite

Diaspora: https://github.com/diaspora/diaspora

Mastdon: https://github.com/tootsuite/mastodon

Peertube: https://github.com/Chocobozzz/PeerTube | https://docs.joinpeertube.org/install-docker

LBRY: https://lbry.com/

##### More Options TBD..

----

### Creator Portal
  - NGINX & PHP-FPM containers running alongside network/service containers on the Creator's instance(s). 
  - Supports creation & management of cluster/nodes via host APIs &/or https://code-ready.github.io/crc/ 

  
#### Web App
PWA: https://ionicframework.com/docs/vue/pwa

#### Mobile App
Ionic Framework: https://ionicframework.com/docs/vue/overview

#### Desktop App
Electron: https://www.electronjs.org/ (cross-platform desktop apps)

----

## Install/Setup Options
Getting started using the Fediverse is VERY simple & straight forward. Creators can use our One-Click/Marketplace app on popular hosts like DigitalOcean, Heroku & Linods to automatically install everything they need. Advanced users may install with Docker (e.g. `docker pull fediverse:10.04`) or simply by pulling this repo & running `docker-compose up -d` 

Anyone who has ever used applications like cPanel & the included One-Click Apps like WordPress will be comfortable with the process. We will provide easy to follow guides, video tutorials, community support/forum & for those who want more hands on support or managed hosting we may provide those services in the future for a fee. (any/all profits should go into philanthropy & supporting the continued development of this project.

1. Digital Ocean
    - Marketplace App https://docs.digitalocean.com/products/app-platform/how-to/create-apps/ 
    - Easy "Deploy to" Button: https://docs.digitalocean.com/products/app-platform/how-to/add-deploy-do-button/
2. Linode
    - Marketplace App https://github.com/linode/Marketplace-Apps
3. Vultr
    - One-Click App: https://www.vultr.com/features/one-click-apps/
4. Heroku
    - Container Registry https://devcenter.heroku.com/articles/container-registry-and-runtime
5. Custom install
    - Downloadable ISO/img
    - Github repo to pull/clone & then use `docker-compose up` to start all services.

## Possible Creator Setup (Digital Ocean option #1) 

1. Goto https://cloud.digitalocean.com/droplets/new
2. Under `Choose an image` select the `Marketplace` tab, search for & select `Fediverse`??
3. Select {min-requirements} & Create Droplet!
4. Navigate to https://NEW_DROPLET_IP 
5. Login with default `user` and `password` & complete the setup wizard.

----

## Dev To-Do
1. ~~Define list/specification of goals/problems to solve.~~ [Fediverse/MetaNet spec sheet](https://docs.google.com/document/d/19svsJhCB9LGgiEq-69DrOMFFDBsNsd812T-nU9VafoU)
2. Determine the best tech stack, libraries & decentralized content networks to use.
3. Create Dockerfile/docker-compose.yml to install/launch networks & services.
    - Setup Docker registry: https://docs.docker.com/registry/deploying/ 
    - Docker Hub account/repo setup: https://docs.docker.com/docker-hub/repos/
    - Become vendor/partner for 1-Click-Apps: https://github.com/digitalocean/marketplace-partners
    - Create `Deploy to..` button: https://docs.digitalocean.com/products/app-platform/how-to/add-deploy-do-button/
4. Build a RESTful JSON API (wrapper for all service APIs + additional Fediverse specific methods)
5. Build packages/plugins for Node.js (Vue store), PHP/composer & others.
6. Create Admin UI used to manage server(s) & content.
7. Create Setup Wizard 
8. Create front-end consumption UI(reader) to serve & display creator content.
9. Create modules/plugins, themes, 3rd party integrations & any other initially required features.


