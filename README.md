## Slate

### How to run -
1. Install Docker for Mac
2. Install Node Module Globally ```npm install -g widdershins```
2. Run ``` docker compose up ```

### Where to start
1. Create a swagger json file or use the existing file saved in ROOT_FOLDER/swagger/swagger.json
2. Generate a Slate MD file by running in root -  ```npm run swag2slate```. This will generate the index.html.md file in ROOT_FOLDER/source/index.html.md

### How to Build -
```shell script
docker run --rm -v $PWD/source:/usr/src/app/source -w /usr/src/app/source -v $PWD/build:/usr/src/app/build slate_app bundle exec middleman build --clean
```

Contributors
--------------------

Slate was built by [Robert Lord](https://lord.io) while interning at [TripIt](https://www.tripit.com/).

Thanks to the following people who have submitted major pull requests:

- [@chrissrogers](https://github.com/chrissrogers)
- [@bootstraponline](https://github.com/bootstraponline)
- [@realityking](https://github.com/realityking)
- [@cvkef](https://github.com/cvkef)

Also, thanks to [Sauce Labs](http://saucelabs.com) for sponsoring the development of the responsive styles.

Special Thanks
--------------------
- [Middleman](https://github.com/middleman/middleman)
- [jquery.tocify.js](https://github.com/gfranko/jquery.tocify.js)
- [middleman-syntax](https://github.com/middleman/middleman-syntax)
- [middleman-gh-pages](https://github.com/edgecase/middleman-gh-pages)
- [Font Awesome](http://fortawesome.github.io/Font-Awesome/)
