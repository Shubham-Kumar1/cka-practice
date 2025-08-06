# 01-pods

## ✅ 1. **Pods** (Realistic Use Cases)

1. Create a single-container Pod named `nginx-pod` running the `nginx:1.21` image, exposing port 80.
2. Create a Pod `multi-container-pod` with 2 containers: one `nginx`, one `busybox`, sharing a volume mounted at `/shared-data`.
3. Create a Pod with a `livenessProbe` using HTTP GET `/healthz` on port 8080 and a `readinessProbe` using `exec` command.
4. Create a Pod with `initContainers` that runs `busybox` and prints `Initialization complete` before main container starts.
5. Create a Pod with `command` and `args` overriding image default entrypoint.
6. Create a Pod running a container that consumes a `ConfigMap` as environment variables.
7. Create a Pod that mounts a Secret as a volume at `/etc/secret-data`.
8. Create a Pod that uses a `hostPath` volume to mount `/data/logs` from the host into the container.
9. Create a Pod with a CPU limit of 500m and memory limit of 256Mi.
10. Create a Pod that runs only if node has the label `type=highmem` using `nodeSelector`.
11. Create a Pod that has a container using lifecycle hooks (postStart and preStop).
12. Create a Pod that uses `imagePullPolicy: Always` and imagePullSecrets to pull from a private registry.
13. Create a Pod in a custom namespace `custom-ns`.
14. Create a Pod that uses a projected volume combining Secret and ConfigMap.
15. Create a Pod with `restartPolicy: OnFailure`.
16. Create a Pod and attach a debug container using `kubectl debug`.
17. Create a Pod with an ephemeral volume using `emptyDir`.
18. Create a Pod with `securityContext` set to run as user `1001` and with `readOnlyRootFilesystem`.
19. Create a Pod with resource `requests` for CPU: 250m and memory: 128Mi.
20. Create a Pod with multiple containers that communicate via localhost.
21. Create a Pod that mounts a downward API volume to access metadata.
22. Create a Pod that writes logs to a file inside the container at `/var/log/app.log`.
23. Create a Pod that uses `terminationGracePeriodSeconds: 30` and observe shutdown behavior.
24. Create a Pod with `volumeMounts.subPath` to mount part of a volume.
25. Create a Pod with a startupProbe to delay liveness checks.
