# gitlab-group

A small convenience script to clone/pull complete groups and subgroups, install npm packages in each projects and download artifacts from each projects.

Tested with

- [X] Gitlab 14 / 15
- [X] MacOs 12.14 (Monterey)

## Prerequisites

The following tools must be installed

- curl - (`brew install curl`)
- jq  - (`brew install jq`)

The script needs a GITLAB url and a personal access token to fetch information in GITLAB. These can be added either via the Enviornment variables.

```shell
export GITLAB_TOKEN="<token>"
export GITLAB_URL="<url>"
```

or set both variables in the beginng of the script by uncommenting and filling following lines:

```shell
#GITLAB_TOKEN="<token>"
#GITLAB_URL="<url>"
```

## Usage

```shell
gitlab-group [options] <group_no>
```

Options are:

|Parameter | Description |
|-|-|
|-g|will clone/pull all projects in groups and subgroups|
|-n|will install npm packages in each projects (npm install)|
|-o|will generate for SAP cap subprojects an openapi.json file|
|-a \<branch\> \<job-name\> |will download artifacts from each projects (gitlab-artifact)|

## Support KDC LAB

If it helps you in any way, We would appreciate any support. A support can be an idea, an improvement or a pull request.

If you want to support [KDC LAB](https://github.com/kdc-lab/) with money, you can do it in the form of [donations](https://paypal.me/kdclab) . We will use all donations to fund our assembly costs or donate it to other open source projects we use.

## License

[MIT](http://opensource.org/licenses/MIT) License

Copyright (c) 2021 KDC LAB / [de-posthac](https://github.com/de-posthac)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
