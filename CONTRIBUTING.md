## Grant of License

By contributing material to this repository ("Contribution"),
you hereby agree to license your Contribution under the
[Creative Commons Attribution License (CC-BY 3.0)][cc-by], and to
include the appropriate copyright notice required by the license.

You represent that that you are legally entitled to grant the above license. If
your employer(s) has rights to the intellectual property that you create that
includes your Contributions, you represent that you have received permission to
make Contributions on behalf of that employer and that your employer has waived
such rights for your Contributions to W3C.

## Disclaimer

All content from this repository is provided as is, and W3C makes no
representations or warranties, express or implied, including, but not limited
to, warranties of merchantability, fitness for a particular purpose,
non-infringement, or title; nor that the contents of this repository are
suitable for any purpose.

***

## Build tool

This website is currently built using [GitHub Pages][gh-pages] which itself
relies on [Jekyll][jekyll]. This automatically transforms the content of this
repository into a [static website hosted on GitHub][serviceworker-org].

### Running Jekyll locally

Installing the [same version of Jekyll][install-jekyll] used by GitHub Pages
along with all of its dependencies is a one liner. From the project's directory,
just run:

    $  gem install github-pages

If you are running Xcode 5.1 or over and get the following error when installing,

    clang: error: unknown argument: '-multiply_definedsuppress' [-Wunused-command-line-argument-hard-error-in-future]

this is [a known issue][jekyll-clang-bug] and you will need to install jekyll
with the following command. (You may need to do this from a superuser shell.)

    $ ARCHFLAGS=-Wno-error=unused-command-line-argument-hard-error-in-future gem install github-pages

Once installed, launch Jekyll from the command line:

    $ jekyll serve --watch

and navigate your browser to `http://localhost:4000`. Modifications to the
source code get automatically picked-up and displayed on page refresh.

## Resources

Each resource (slides, presentations, articles, etc.) gets an entry in the
`_post` directory. Please follow file naming conventions as described for blog
posts in the [online documentation][jekyll-blog].

All resource posts must be located in the `_posts` directory and must use the `resources`
template (which should be specified in the [YAML front-matter][front-matter]).

resource posts can be of three different categories: `slides`, `presentation`,
and `article`. Categories are added using [YAML front-matter][front-matter].

Resources will will have data automatically pulled from the `people` database
located in `/data/people.yml` in order to populate the "about the
author section".

## Contribution workflow

Contributions should follow the standard open source GitHub workflow (fork
the repository, work off topic-branches, send atomic commits as pull requests,
and get them reviewed by a peer).

Thanks for your help!

[cc-by]: https://creativecommons.org/licenses/by/3.0/
[front-matter]: http://jekyllrb.com/docs/frontmatter/
[gh-pages]: http://pages.github.com/
[install-jekyll]: https://help.github.com/articles/using-jekyll-with-pages
[jekyll]: http://jekyllrb.com/
[jekyll-blog]: http://jekyllrb.com/docs/posts/
[jekyll-clang-bug]: https://github.com/jekyll/jekyll/issues/2125
[serviceworker-org]: http://serviceworker.org
[yaml]: http://www.yaml.org/
