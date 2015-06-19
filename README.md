# sense-go

> Library to easily handle validation, deployment, packaging and testing of Qlik Sense Visualization Extensions.

**Note: This library is in development and not ready to use, yet**

## Purpose

Main purpose of this library is to provide a framework to easily

+ validate
+ package
+ deploy and
+ test

**Visualization Extensions** created for Qlik Sense.

The implementation is a based on the deployment functionality in the [Yeoman Generator for Visualization Extensions](https://github.com/stefanwalther/generator-qsExtension).

The main reason behind creating this library is that I am creating a lot of different visualization extensions for Qlik Sense, but in any of these projects I include some kind of deployment system (so far always using grunt). If I have to make changes to the general deployment approach I have to change every single visualization extension repository, which is not really ideal. So introducing this library centralizes the deployment needs and allows me to re-use a central approach.

Technically speaking sense-go is just a collection of configurable gulp tasks which can be easily re-used when developing your Qlik Sense visualization extensions.

## Deployment

### Less

Transpile Less files to CSS.

+ less

**Options:**

+ less
  - src - source mask
  - dest - destination
  - cwd - Current working directory

**Example:**

### Clean local local deployment directory

**Options:**

+ clean
  - src
  - cwd

### Upload to Qlik Sense server

Upload the zipped visualization extension to a Qlik Sense server (using the Repository API in behind).

**Options:**

+ upload
  - src
  - cert
  - serverUrl

### Compress

Compress files.

**Options:**

+ compress
  - src
  - dest
  - format
  - password Set a password to protect the .zip file.

### Replace

Replace strings in relevent text files (.js, .txt, .json, .yml, .txt, .css)

### Uglify

(TBC)

### Minify

(TBC)

## Validation

(TBC)

## Roadmap

**Less**

+ [x] Implementation
+ [x] Test
+ [ ] Documentation

## Author

**Stefan Walther**

## License

Copyright © 2015
Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on June 19, 2015._