[Software Architecture](../..) > [Patterns](..) > API Design

---

Patterns of designing remote APIs.
- The [RPC](api-design/rpc) style (remote procedure call) of API design exposes a function or procedure to be called via a network. The words function and procedure have their usual meanings: a function is a query (it returns a result), and a procedure is a command (it causes an effect). RPC-style APIs are generally synchronous (blocking) because an asynchronous API is much more natural to implement in the resource style.
- [Resource](api-design/resource) style APIs are oriented around creating, querying, and modifying notional resources on the remote end. These include document-style SOAP APIs as well as RESTful APIs which are modelled as HTTP resources. Asynchronous APIs are natural to implement in the resource style because the initial invocation can create a resource that represents the status (and result, if appropriate) of the asynchronous operation.
