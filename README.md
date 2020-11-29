Sync at 13/06/2020

### devlopr-jekyll - A Beautiful Jekyll Theme Built for Developers

[![Gem Version](https://badge.fury.io/rb/devlopr.svg)](https://badge.fury.io/rb/devlopr)![workflow-badge](https://github.com/sujaykundu777/devlopr-jekyll/workflows/deploy/badge.svg)
[![Netlify Status](https://api.netlify.com/api/v1/badges/4232ac2b-63e0-4c78-92e0-e95aad5ab8c3/deploy-status)](https://app.netlify.com/sites/devlopr/deploys)
![](https://ruby-gem-downloads-badge.herokuapp.com/devlopr?type=total&color=brightgreen&style=plastic)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)

Just a little something I'm using to jump start a site refresh. I like to think of it as a starter for building your own Jekyll site. I purposely keep the styling minimal and bare to make it easier to add your own flare and markup.
The Theme supports both Light and Dark Style. Highly Customizable and No Hosting or Maintainence Cost is required !

### [Installation Guide](https://devlopr.netlify.app/get-started)

You can easily manage the site using the admin : [http://localhost:4000/admin](http://localhost:4000/admin)


### Demo (Hosted Apps)

#### Features :

## Release Changes :

You can check out the latest changes [here](https://www.buymeacoffee.com/p/57109)

## Using Docker :

Building the Image :

`docker build -t my-devlopr-jekyll-blog .`

Running the container :

`docker run -d -p 4000:4000 -it --volume="$PWD:/srv/jekyll" --name "my_blog" my-devlopr-jekyll-blog:latest jekyll serve --watch`

## Using Docker Compose :

### Development :

You can run the app in development mode : (your changes will be reflected --watch moded)

Serve the site at http://localhost:4000 :

`docker-compose -f docker-compose-dev.yml up --build --remove-orphans`

### Production :

You can run the app in production mode : (your changes will be reflected --watch moded)

Serve the site at http://localhost:4000 :

`docker-compose -f docker-compose-prod.yml up --build --remove-orphans`

Stop the app :
`docker-compose -f docker-compose-prod.yml down`
Once everything is good and ready to go live -

`docker-compose -f docker-compose-prod.yml up --build --detach`

## Contributors:


### Backers

Thanks to all our Backers ! 🙏 [Become a Backer](https://opencollective.com/devlopr-jekyll#backer)

## Licence

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT). You can do anything you want, including projects for your clients, as long as you mention an attribution back (credit links in footer). See the [Licence](https://github.com/sujaykundu777/devlopr-jekyll/blob/master/LICENSE) file

I understand that sometimes footer links or any links to external websites are not convenient, so you have the option to remove credits/footer links by becoming a [Backer](https://opencollective.com/devlopr-jekyll#backer).
