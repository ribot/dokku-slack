# Dokku Slack

Dokku Slack is a plugin for [Dokku](https://github.com/progrium/dokku) that notifies [Slack](http://www.slack.com) of deployments.

## Installation

```sh
git clone https://github.com/ribot/dokku-slack.git /var/lib/dokku/plugins/dokku-slack
```

## Configuration

Edit `/home/dokku/dokkurc` or `/etc/slack`

```sh
export SLACK_NOTIFY=1
export SLACK_DOMAIN=<domain>
export SLACK_TOKEN=<token>
export SLACK_USERNAME='Dokku'
export SLACK_CHANNEL=dokku #default_channel
```

The domain is the subdomain part of the URL use use to get to the Slack webapp. For example for `http://ribot.slack.com/` it's `ribot`.

### Using app specific channel

```sh
dokku config:set $APP SLACK_CHANNEL=your_channel
```

You can send notification to app specific channel.

## License

The MIT License (MIT)

Copyright (c) 2014 ribot

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
