### kassett-python-cicd

I build this Github Actions workflow because it seemed that I was performing the same few steps
over and over again when publishing a Python package.
In this workflow you have the ability to do a few useful things:
* Assume an AWS Role
* Generate environment variables using AWS secrets
* Run test command
* Publish a Python package using Twine / Poetry

Suggested usage
1. Build a Makefile with targets that
   1. install dependencies
   2. run tests
2. Pass those Makefile targets into workflow 