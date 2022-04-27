[Software Architecture](../../..) > [Patterns](../..) > [API Design](..) > Resource Style API

---

# Resource Style API

Resource style APIs are oriented around creating, querying, and modifying notional resources on the remote end. These include document-style SOAP APIs as well as RESTful APIs which are modelled as HTTP resources. Asynchronous APIs are natural to implement in the resource style because the initial invocation can create a resource that represents the status (and result, if appropriate) of the asynchronous operation.
