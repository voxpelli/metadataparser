# Metadataparser

[![Build Status](https://travis-ci.org/voxpelli/metadataparser.svg?branch=master)](https://travis-ci.org/voxpelli/metadataparser)
[![Coverage Status](https://coveralls.io/repos/github/voxpelli/metadataparser/badge.svg?branch=master)](https://coveralls.io/github/voxpelli/metadataparser?branch=master)
[![Dependency Status](https://gemnasium.com/voxpelli/metadataparser.svg)](https://gemnasium.com/voxpelli/metadataparser)
[![js-semistandard-style](https://img.shields.io/badge/code%20style-semistandard-brightgreen.svg?style=flat)](https://github.com/Flet/semistandard)

### The flow to update the Lambda method

1. Do a `yarn install` using [Yarn](https://yarnpkg.com/) or a `npm install`
2. When the dependencies has been installed, zip the folder into a zip-file where the folder itself is included. When Amazon unzips it the handler should be `metadataparser/index.fetchBatch`. One way to do this is to right-click the folder on OS X and chose to *compress* it.
3. Go to the AWS Console for your Lambda job and upload the zip-file.
4. Done. It can take a short while for the new code to reach all the Lambda servers, but that's to be expected and something that happens on our own infrastructure as well.
