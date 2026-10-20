# partner-demo

Minimal example for a "one commit, two clusters" Fleet demo: a Deployment `web`
(2 replicas) plus a Service, in namespace `partner-demo`.

It runs as non-root on port 8080 with a RuntimeDefault seccomp profile and all
capabilities dropped, so it is admitted under Pod Security `restricted` without
any namespace exemption.
