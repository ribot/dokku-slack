<img src="https://cdn.rawgit.com/crisward/dokku-slack/master/dokku-slack.svg" height="140"/>

Dokku Slack is a plugin for [Dokku](https://github.com/progrium/dokku) that notifies [Slack](http://www.slack.com) of deployments.

## Installation

```sh
# dokku 0.3.26
$ sudo git clone https://github.com/ribot/dokku-slack /var/lib/dokku/plugins/slack

# dokku 0.4+
$ sudo dokku plugin:install https://github.com/ribot/dokku-slack.git slack
```

## Commands

```sh
$ dokku help
    slack:help                                      Show Only Slack Help
    slack:set <app> <webhook_url>                   Set Slack WebHook URL
    slack:set <webhook_url>                         Set same WebHook URL for all Apps
    slack:clear <app>                               Clears Slack WebHook URL
    slack:get <app>                                 Display Slack WebHook URL
```

To get **WebHook URL** you need to create a new
[**Incoming WebHook integration**](https://slack.com/services/new/incoming-webhook).

## Credit

Logo courtesy of the [Noun Project](https://thenounproject.com/)

## License

The MIT License (MIT)

Copyright (c) 2015 ribot

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
