# Nipraxis pages

This is the repository corresponding to the main pages for the course,
currently at <https://nipraxis.org>.

Look at the `gh-pages` branch for the source for the web-pages.  If you want to edit the web pages, checkout that branch and work there.

This branch is for any other files relating the course as a whole.  Files for
particular iterations go in their respective repositories - e.g.
<https://github.com/nipraxis/spring-2022>.

## Page and repository structure

We will call the Nipraxis course as a whole - the *course*.

Any particular iteration of the course is an *iteration*. For example, we will
have a Nipraxis iteration in Spring 2022 and in Fall 2022.

The course has a repository - this one.

Each iteration has its own repository.

All repositories (course and iteration repositories) have at least two
branches:

* `main` : for files related to the course or iteration.
* `gh-pages` : for web pages appearing at <https://nipraxis.org> (the course
  site) or at (e.g.) <https://nipraxis.org/spring-2022> (an iteration site).

We use versions of the [JustTheClass
template](https://github.com/kevinlin1/just-the-class) for the web pages in
`gh-pages` branches.  These are Jekyll sites, so Github will render these to
web pages automatically on push.  The `gh-pages` branch is therefore the
*source* for the web pages.  Edit files in that branch to change any web page
content.

Meanwhile the `main` branch may have homework, labs or other useful files for
the course, or course iteration.

The general structure comes from the one I found for the [DS-100
repositories](https://github.com/DS-100).

## DNS setup

See the [Github instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

Specifically, the `gh-pages` branch here has a `CNAME` file with contents `nipraxis.org`.   The `textbook` repo `gh-pages` branch has `CNAME` file with `textbook.nipraxis.org`.  My DNS provider has the following CNAME records:

Host record Points to
=========== =========
@           nipraxis.github.io
www         nipraxis.github.io
textbook    nipraxis.org

I needed to set up both `@` and `www` records to get the original top-level
domain working.  See the Github page custom domain instructions above.
