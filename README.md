# Hugo DFD Demo Site Theme

A theme for [Hugo](https://gohugo.io) module demo sites by [Daniel F. Dickinson](https://www.danielfdickinson.ca).

## Netlify Status

TBD

## Features

* Hugo module
* exampleSite (for demo deploys and/or documentation)
* Netlify-ready
  * Cache resources folder (exampleSite)
  * HTML Validation
  * Check internal links
  * HTML Minification

## Using the Theme
1. Create a hugo site
   ```
   hugo new site hugo-test-dfd-demo-site-theme
   cd hugo-test-dfd-demo-site-theme
   ```
### Using Hugo Modules (preferred)

1. Initialize the Hugo module system: ``hugo mod init github.com/<your_user>/<your_project>`` (assuming you are using github, of course).
2. Import the theme in your ``config.toml``
   ```
   [module]
     [[module.imports]]
        path = "github.com/danielfdickinson/hugo-dfd-demo-site-theme"
   ```
3. Change back to the site directory
4. Get the module
   ```
   hugo mod get github.com/danielfdickinson/hugo-dfd-demo-site-theme
   hugo mod tidy
   ```
5. To test the result, run the local Hugo server
   ```
   hugo server -b http://localhost:1313/
   ```
### Using downloaded copy of the theme (e.g. ZIP from the Git repo)

1. Make a themes directory and switch to it
   ```
   mkdir themes
   cd themes
   ```

2. Obtain a copy of the latest development version of the theme e.g. ([a theme Zip file from the Git repo](https://github.com/danielfdickinson/hugo-dfd-demo-site-theme/archive/refs/head/main.zip))
3. Copy/extract the theme into hugo-dfd-demo-site-theme in the themes directory
4. Change back to the site directory
5. To test the result, run the local Hugo server
   ```
   hugo server -t hugo-dfd-demo-site-theme -b http://localhost:1313/
   ```
### Using git submodules (deprecated)

1. Make a themes directory and switch to it.
   ```
   mkdir themes
   cd themes
   ```

2. In the themes directory, add hugo-dfd-demo-site-theme as a submodule
   ```
   git submodule add -f https://github.com/danielfdickinson/hugo-dfd-demo-site-theme
   ```
3. Change back to the site directory
4. To test the result, run the local Hugo server
   ```
   hugo server -t hugo-dfd-demo-site-theme -b http://localhost:1313/
   ```

 Enjoy!
