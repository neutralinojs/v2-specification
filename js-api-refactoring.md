## Params to Interfaces

v1.x implementation

The client API (aka `neutralino.js`) is having parameters-based methods. The plan is to refactor all methods with an interface. 

Example:

`Neutralino.debug.log(string type, string message, success)`

v2.x implementation

`Neutralino.debug.log(LoggerOptions options)`

```
LoggerOptions;
{
  string messageType;
  string messageContent;
  function onSuccess;
  function onError
}
```

## Handle Server errors

v1.x implementation

If there is an error thrown from Neutralino server, the client library will trigger the success callback because 
the communication was success with the server.

v2.x implementation

If there is an error thrown from the server, `onError` callback will be triggered.
