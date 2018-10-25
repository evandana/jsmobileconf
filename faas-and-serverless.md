# The FaaS and the Serverless

Simon MacDonald (@macdonst)

puns! (not jokes, because they're not good)


## Summary

- Stateless (no dependency other than input)
- Pure (no side effects)
- One task per function (use `compose` if necessary)
- Use events to fire off sequences of functions


### Gotchas

- No caching!
    - Because function spun up and torn down at end of function
- Logging?
    - Offered per vendor
- Cloud functions are not in memory, may require some spin up time
    - Quick for Node (and other interpreted languages)
    - Slow for Java (and other compiled languages)
- Security?
    - HIPAA compliance possible per vendor
- Benefit for mid-tier use case
    - Unbounded scaling
- Harder to debug series of functions instead of monolith



## FaaS

### Do one thing, and do it well

- Fetch
- Process
- Transform
- UI

### Compose

- `return compose(func1, func2, func3)`

### Events (lamda)

- Git commit
- Database action
- cron job
- Blob storage
- Analytics


## Serverless

### Products

- IBM BlueMix Openwisk
- Exert cloud functions
- AWS Lamda
- GCP Cloud Functions

### Layers

- Code (FaaS)
- Containers (SaaS/PaaS)
- Infrastructure (IaaS)
- Scaling


## Convert SPA to Serverless

- Static assets (HTML, CSS, JS) => CDN
- Routes => Cloud Functions