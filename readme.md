npm init

npm i @11ty/eleventy @11ty/eleventy-cache-assets @11ty/eleventy-img @11ty/eleventy-plugin-syntaxhighlight autoprefixer cross-env cssnano eleventy-plugin-time-to-read markdown-it markdown-it-attrs netlify-plugin-cache npm-run-all postcss postcss-cli sass

Scripts for package json
"watch:sass": "sass  --no-source-map --watch src/sass:_site/css",
    "watch:eleventy": "eleventy --serve",
    "build:sass": "sass  --no-source-map src/sass:_site/css",
    "build:eleventy": "eleventy",
    "postbuild": "postcss _site/css/*.css -u autoprefixer cssnano -r --no-map",
    "start": "npm-run-all build:sass --parallel watch:*",
    "build": "npm-run-all build:sass build:eleventy"


setup gitignore

