Cloud Foundry Hugo Buildpack
===

This is a [Cloud Foundry buildpack](http://docs.cloudfoundry.org/buildpacks/)
for sites powered by [Hugo](https://github.com/spf13/hugo).

This buildpack is a fork of the Heroku Hugo buildpack found [here](https://github.com/roperzh/heroku-buildpack-hugo).

Important notes
===
This buildpack executes the Hugo [server](https://gohugo.io/commands/hugo_server/)
command which builds and serves the site.

The theme for the site must be specified in the Hugo [configuration file](https://gohugo.io/overview/configuration/).

***Example***

```text
theme = "purehugo"
```

To bump the Hugo version just add a `.hugo-version` file in the root directory
of your site with the target Hugo release version number.

***Example .hugo-version file contents***

```text
0.17
```

Usage
===

Simply push a Hugo site to Bluemix using this buildpack:

```bash
$ cf push "${CF_APP}" -b https://hub.jazz.net/git/mschimko/hugo-buildpack
```

Contributing
===

1- Fork the project

2- Submit a Pull Request

License
===

The MIT License (MIT)

Copyright (c) 2015 Roberto Dip

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
