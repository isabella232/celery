# DEPRECATED

This image is officially deprecated in favor of [the standard `python` image](https://hub.docker.com/_/python/), and will receive no further updates after 2017-06-01 (Jun 01, 2017). Please adjust your usage accordingly.

See the discussion in [docker-library/celery#1](https://github.com/docker-library/celery/issues/1#issuecomment-287655769) and [docker-library/celery#12](https://github.com/docker-library/celery/issues/12) for more details.

In most cases, using this image required re-installation of application dependencies, so for most applications it ends up being much cleaner to simply install Celery in the application container, and run it via a second command.

See [the way the `sentry` image handles running a Celery beat and workers](https://github.com/docker-library/docs/blob/d328e02359c6fc9a7f1f3c59efa2893f63e667e4/sentry/README.md#how-to-setup-a-full-sentry-instance) for a concrete example of this pattern being employed (`docker run -d --name sentry-cron ... sentry run cron` and `docker run -d --name sentry-worker-1 ... sentry run worker`).

# About this Repo

This is the Git repo of the Docker [official image](https://docs.docker.com/docker-hub/official_repos/) for [celery](https://registry.hub.docker.com/_/celery/). See [the Docker Hub page](https://registry.hub.docker.com/_/celery/) for the full readme on how to use this Docker image and for information regarding contributing and issues.

The full readme is generated over in [docker-library/docs](https://github.com/docker-library/docs), specifically in [docker-library/docs/celery](https://github.com/docker-library/docs/tree/master/celery).

See a change merged here that doesn't show up on the Docker Hub yet? Check [the "library/celery" manifest file in the docker-library/official-images repo](https://github.com/docker-library/official-images/blob/master/library/celery), especially [PRs with the "library/celery" label on that repo](https://github.com/docker-library/official-images/labels/library%2Fcelery). For more information about the official images process, see the [docker-library/official-images readme](https://github.com/docker-library/official-images/blob/master/README.md).

---

-	[Travis CI:  
	![build status badge](https://img.shields.io/travis/docker-library/celery/master.svg)](https://travis-ci.org/docker-library/celery/branches)
-	[Automated `update.sh`:  
	![build status badge](https://doi-janky.infosiftr.net/job/update.sh/job/celery/badge/icon)](https://doi-janky.infosiftr.net/job/update.sh/job/celery)

<!-- THIS FILE IS GENERATED BY https://github.com/docker-library/docs/blob/master/generate-repo-stub-readme.sh -->
