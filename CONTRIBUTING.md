# Contributing guide

**Want to contribute? Great!** 
We try to make it easy, and all contributions, even the smaller ones, are more than welcome.
This includes bug reports, fixes, documentation, examples... 
But first, read this page (including the small print at the end).

## Build and run locally

*Note:*
The `jekyll-github-metadata` plugin will perform some API requests to GitHub, which can lead to rate-limiting warnings.
To avoid seeing these, create a GitHub personal access token with `public_repo` scope, and set it as the value of the `JEKYLL_GITHUB_TOKEN` environment variable.


Building and running locally requires Ruby and bundler.
You can either bring your own, or use the Jekyll container image.

### Bring your own Ruby & bundler

```bash
bundle install
bundle exec jekyll serve --incremental
```

### Using a container image with Podman or Docker

```bash
docker run -ti --rm \
    -v .:/srv/jekyll \
    -p 4000:4000 \
    -e JEKYLL_ROOTLESS=1 \
    -e JEKYLL_GITHUB_TOKEN \
    docker.io/jekyll/jekyll \
    jekyll serve --incremental
```

## Legal

All original contributions to this repo are licensed under the
[ASL - Apache License](https://www.apache.org/licenses/LICENSE-2.0),
version 2.0 or later, or, if another license is specified as governing the file or directory being
modified, such other license.

All contributions are subject to the [Developer Certificate of Origin (DCO)](https://developercertificate.org/).
The DCO text is also included verbatim in the [dco.txt](dco.txt) file in the root directory of the repository.

## Reporting an issue

This project uses GitHub issues to manage the issues. Open an issue directly in GitHub.

If you believe you found a bug, and it's likely possible, please indicate a way to reproduce it, what you are seeing and what you would expect to see.

### Code reviews

All submissions, including submissions by project members, need to be reviewed by at least one committer before being merged.

[GitHub Pull Request Review Process](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews) is followed for every pull request.
