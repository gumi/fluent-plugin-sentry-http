# fluent-plugin-sentry-http

[fluentd](http://fluentd.org) input plugin that receive exceptions from [Sentry Clients](https://github.com/getsentry).

[![Build Status](https://travis-ci.org/gumi/fluent-plugin-sentry-http.svg?branch=master)](https://travis-ci.org/gumi/fluent-plugin-sentry-http)
[![Code Climate](https://codeclimate.com/github/gumi/fluent-plugin-sentry-http/badges/gpa.svg)](https://codeclimate.com/github/gumi/fluent-plugin-sentry-http)

## Installation

Install with gem or fluent-gem command as:

```
# for fluentd
$ gem install fluent-plugin-sentry-http

# for td-agent
$ sudo /usr/lib64/fluent/ruby/bin/fluent-gem install fluent-plugin-sentry-http
```

## Component

### SentryHttpInput

Plugin to accept exception input from [Sentry Clients](https://github.com/getsentry).

#### Configuration

```
<source>
  type sentry_http
  port 8888
  bind 0.0.0.0
  <project 999>
    tag sentry.egg
    key aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
    secret bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
  </project>
</source>
```

## Copyright

- Copyright
  - Copyright (C) 2016- gumi Inc.
- License
  - Apache License, Version 2.0
