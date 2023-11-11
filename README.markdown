### Generating the website locally ###
* You will need [Jekyll to generate the website](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll)
* Make sure that your [Github Pages gem is up to date](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll#updating-the-github-pages-gem)
* Run `make`

### Checklist for deployment ###

#### Visual check ###
* Run `make` to generate the website
* Go to the generated URL (default URL is [http://127.0.0.1:4000](http://127.0.0.1:4000))
* Check the changes you have made

#### Check links ####
Run `wget` locally to check for broken links using the following steps:

* Run `make` to generate the website
* Crawl the website using: `wget --spider -r -nd -nv  -l 0 -o run.log http://127.0.0.1:4000/`
* Check the log from `Jekyll` and `run.log` for any broken links.

If you want to check for broken links in the deployed website, you can use the following command:
`wget --spider -H --domains whilab.org -r -nd -nv  -l 0 -o  run.log -w 1 whilab.org`

You can then check `run.log` to find any broken links.
