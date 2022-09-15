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

git init

Quick setup — if you’ve done this kind of thing before
or	
git@github.com:vinodkanneganti/personalsite.git
Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

…or create a new repository on the command line
echo "# personalsite" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:vinodkanneganti/personalsite.git
git push -u origin main
…or push an existing repository from the command line
git remote add origin git@github.com:vinodkanneganti/personalsite.git
git branch -M main
git push -u origin main
…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.

