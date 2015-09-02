node-squarespace-logger
=======================

> Shared logging utility for node-squarespace- modules.


### Installation
```shell
npm install node-squarespace-logger
```

#### Updating
```shell
npm update node-squarespace-logger
```



### Usage

```javascript
var sqsLogger = require( "node-squarespace-logger" );

// Log some useful stuff
sqsLogger.log( context, message );

// Silence the logger
sqsLogger.silence();

// Pass your logger around to child modules to retain the silence
var myModule = require( "./my-module" )( sqsLogger );

// or like this
var myModule = require( "./my-module" );
myModule.setLogger( sqsLogger );
```

These are the context types for the logger
- info ( white )
- warn ( yellow )
- error ( red )
- server ( magenta )
- cache ( green )
- template ( cyan )



### Pull Requests
1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
