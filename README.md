scaffold
========

A scaffold for Static and Wordpress web projects.

## Resources

* HTML 5
* Sass (CSS 3)
* CoffeeScript (JavaScript)
* Grunt tasks:
  * Compile CoffeeScript
  * Compile Sass
  * Coffelint
  * JShint
  * YUI Compressor: minify JavaScript and CSS
  * `grunt-shell` runs after everything to execute `rsync` to send files as specified in the `config`, with `deployit.sh` script
  * Docco for documentation of CoffeeScript
=======
A scaffold for websites -- static and PHP based (WordPress).

## Goals

- [x] HTML 5
- [x] Stylus (CSS 3)
- [x] CoffeeScript (JavaScript)
- [x] Gulp
- [x] Grid: [jeet](http://jeet.gs)
- [x] [Axis](http://axis.netlify.com/)
- [x] Media queries: [rupture](http://jenius.github.io/rupture/)
- [x] Compile `.coffee`, `.styl`
- [x] Minify `.js`, `.css`, `.html`, `.php` (html, php: `[pagename]-dev.html` or `[pagename]-dev.php` to `[pagename].html` or `[pagename.php]`)
- [x] Optimize images (it is saved in `images/public`)
- [x] Live reload
- [x] Docco to document CoffeeScript
- [x] Lint `.coffee`
- [x] **Optional** deploy with ShellScript (you should to configure your `ssh` access to not having to enter the password every deploy -- *this does not provide here*)
- [ ] WordPress theme scaffold
- [ ] Tests

## Install

```
git clone https://github.com/marcker/scaffold
mv scaffold YourProjectName
cd YourProjectName
rm -rfv .git
git init # optional
```

*Uncomment the extensions that you wish in the `.gitignore`*
=======
*You should to uncomment the extensions that you want in the `.gitignore`*

### Static

For static websites.

```
cd static
npm install && npm install jeet
gulp
```

#### Deploy

```
cd deploy
```

Add to file **config**: `../FOLDER_OR_FILE`, `USER@IP`, `DESTINATION` (whitespace and comma separated). After:

```
chmod +x deployit.sh
./deployit.sh
```

### Wordpress

* Coming soon
