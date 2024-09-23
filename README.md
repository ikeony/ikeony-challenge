However, from my experience with node deployments, usually an environment file could be used (one for dev, staging/qa, prod), or some way to load different environment variables to production. 

Test files would be added (either for unit testing or integration testing with Jest).

A CI/CD pipeline would run through these test cases to ensure nothing was broken, and then a docker image would be created.

This docker imaged would be deployed using an orchestration system like Kubernetes.
