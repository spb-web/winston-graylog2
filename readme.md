# winston-graylog2

A graylog2 transport for [winston][0]. Inspired [winston-mail][1] transport.

## Installation

## Usage
``` js
  var winston = require('winston');

  //
  // Requiring `winston-graylog2` will expose
  // `winston.transports.Graylog2`
  //

  winston.add(require('./winston-graylog2.js').Graylog2, options);

```

Options are the following, `to` and `host` are required:

* __level:__ Level of messages this transport should log. (default: info)
* __silent:__ Boolean flag indicating whether to suppress output. (default: false)

* __graylogHost:__ IP address or hostname of the graylog2 server. (default: localhost)
* __graylogPort:__ Port to send messages to on the graylog2 server. (default: 12201)
* __graylogHostname:__ The hostname associated with graylog2 messages. (default: require('os').hostname())
* __graylogFacility:__ The graylog2 facility to send log messages.. (default: nodejs)

[0]: https://github.com/flatiron/winston
[1]: https://github.com/wavded/winston-mail