### Generating the website locally ###
* You will need [Jekyll to generate the website](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll)
* Make sure that your [Github Pages gem is up to date](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll#updating-the-github-pages-gem)
	* You can run `make bundle` to ensure that the gem is updated.
* Run `make` to generate the website ([http://127.0.0.1:4000](http://127.0.0.1:4000))

### Checklist for deployment ###

#### Spell ####
Please run `make spell` to check for spelling. If you are not familiar with `aspell`, feel free to use other spell checkers.

#### Visual check ###
Please make sure that there are no obvious visual inconsistencies in the added content. 

* Run `make` to generate the website
* Go to the generated URL (default URL is [http://127.0.0.1:4000](http://127.0.0.1:4000))
* Check the changes you have made

#### Check links ####

Please follow the following two steps to ensure there are no broken links.

##### link validation by default #####
Internal links should be validated by default. That is, when linking to any internal
urls, you should use the `link` tag (see [Jekyll documentation](https://jekyllrb.com/docs/liquid/tags/#links)).
This will ensure that broken links are identified during the site generation step.

##### wget to identify broken links #####

Run `wget` locally to check for broken links using the following steps:

* Run `make` to generate the website
* On a separate terminal, run `make link`
* Check `wget-run.log` for any broken links.

If you want to check for broken links in the deployed website, you can use the following command:
`wget --spider -H --domains whilab.org -r -nd -nv  -l 0 -o  run.log -w 1 whilab.org`. You can then check `run.log` to find any broken links.
