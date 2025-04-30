# 8173.uk Redirect Service

Going to 8173.uk or any of its subpaths will redirect to a different page, either one under our website gearzero.uk or anywhere else on the web. Practically, it's our own URL shortening service. Technically, it's a very simple static site (so it can be hosted as static files without a backend needed). Right now, the URLs aren't private but they could be made so by making the code repository private.

## Adding a link

Let's say you want the URL `https://8173.uk/foobar` to redirect to `https://gearzero.uk/the-long-time-weve-spent-fooing-and-baring`. You would do this the following way:
* Create a new folder called `foobar`.
* Create a file called `index.html` inside the folder, and copy the contents of the root folder's `index.html` into it. Your access rights probably require you to make a fork of this repository; the Git forge (right now, GitHub) will show you how to.
* Change `href="https://gearzero.uk"` to `href="https://gearzero.uk/the-long-time-weve-spent-fooing-and-baring"`.
* Save, commit, and open a pull/merge request with your changes (the forge also guides you here).
* Once the changes have been merged, the link will work!

## Advanced options

### I want a source link like `https://8173.uk/foo/bar`, perhaps for organisation purposes

Create a folder `foo` in the root of this repository, then a folder `bar` inside `foo`, then the `index.html` file inside this `bar` folder.
