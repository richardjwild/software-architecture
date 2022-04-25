# RPC Style APIs

The RPC style (remote procedure call) of API design exposes a function or procedure to be called via a network. The words function and procedure have their usual meanings: a function is a query (it returns a result), and a procedure is a command (it causes an effect). RPC-style APIs are generally synchronous (blocking) because an asynchronous API is much more natural to implement in the resource style.
