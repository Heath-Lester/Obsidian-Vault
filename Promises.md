
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise

>The **`Promise`** object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.


A `Promise` is in one of these states:

- _pending_: initial state, neither fulfilled nor rejected.
- _fulfilled_: meaning that the operation was completed successfully.
- _rejected_: meaning that the operation failed.

Promises are chainable with their `then`, `catch`, and `finally` methods.