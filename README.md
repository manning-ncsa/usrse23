# The US-RSE Association Conference 2023 (USRSECon23)

This repo is website landing page for the US-RSE Association Conference 2023,
happening October 16-18 in Chicago, IL.

## Previewing the Site Locally

To preview the site locally, you'll need to [install jekyll](https://jekyllrb.com/docs/installation/)
Then go to the root of the directory and run (only needed once):

```bash
$ bundle install
```

Then run 

```bash
$ jekyll serve
# or
$ bundle exec jekyll serve
```

and open your browser to <http://localhost:4000>.

If you are having trouble try `rm -rf _site`, followed by `bundle update`,
then `bundle exec jekyll serve`.


## Previewing the Site Locally using Docker

Build the container image:

```bash
docker build -t us-rse-website:latest .
```

Run the container, forwarding port 4000 to allow viewing the website at http://127.0.0.1:4000.

```bash
docker run --rm -it -p 4000:4000 us-rse-website:latest
```
