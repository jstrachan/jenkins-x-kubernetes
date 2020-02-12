# Reusable ChatOps Contexts

This directory contains reusable contexts you can enable on your `Scheduler` resource to add the pipeline to your repository without having to write a new `jenkins-x-$context.yml` file.

i.e. its a way to share reusable pipelines across git repositories.

So if you add the `go-lint` context to your `Scheduler` it will be effectively like you copied the [go-lint/jenkins-x.yml](go-lint/jenkins-x.yml) file into the `jenkins-x-go-lint.yml` file in all of your source repositories

## Overriding the context

If you add, say, the `go-lint` reusable context to all your `Scheduler` resources you may want to override things in one of your repositories. If so just create a `jenkins-x-go-lint.yml` file in your source repository and use the usual overriding mechanism in Jenkins X Pipelines
