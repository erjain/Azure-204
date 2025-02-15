# Azure-204
## Things to remember
1. Containers in the container group are always restarted with an Always policy in effect, regardless of their exit code. Running containers using a managed identity would simplify the access to external Azure resources but doing so has no effect on when a container restarts. When the processes in the container fail (terminating with a nonzero exit code), they will not restart and will only run once at most. Init containers are meant to perform initialization logic for app containers, running to completion before the application containers start.

2. The WEBSITE_LOAD_CERTIFICATES app setting makes the specified certificates accessible to Windows or Linux custom containers as files. 
