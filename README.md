# What is a Cartridge?

A Cartridge is a set of resources that are loaded into the Platform for a particular project. They may contain anything from a simple reference implementation for a technology to a set of best practice examples for building, deploying, and managing a technology stack that can be used by a project.

This cartridge consists of source code repositories and jenkins jobs.

## Pre-requisite
* Configure the Sonar server authentication token in Manage Jenkins > Configure System > SonarQube servers.

## Source code repositories

Cartridge loads the source code repositories

* [ngx-admin](https://github.com/victornc83/ngx-admin.git)
* [adop-cartridge-npm-regression-tests](https://github.com/victornc83/adop-cartridge-npm-regression-tests)
* [adop-cartridge-npm-environment-template](https://github.com/victornc83/adop-cartridge-npm-environment-template)

## Jenkins Jobs

This cartridge generates the jenkins jobs and pipeline views to -

* Provision the environment.
* Creating a Pipeline job which references a Jenkinsfile living in the [ngx-admin](https://github.com/victornc83/ngx-admingit) repository which is responsible for:
  * Build the source code from sprint ngx-admin repository.
  * Running unit tests on the compiled code.
  * Running sonar analysis on the code.
  * Deploy to an environment.
  * Run regression tests on deployed petclinic application.

# License
Please view [license information](LICENSE.md) for the software contained on this image.

## Documentation
Documentation will be captured within this README.md and this repository's Wiki.

## Issues
If you have any problems with or questions about this image, please contact us through a [GitHub issue](https://github.com/victornc83/adop-cartridge-npm-pipeline/issues).

## Contribute
You are invited to contribute new features, fixes, or updates, large or small; we are always thrilled to receive pull requests, and do our best to process them as fast as we can.



