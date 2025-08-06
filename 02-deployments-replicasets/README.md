# 02-deployments-replicasets

1. Create a Deployment `web-deploy` with 3 replicas running `nginx:1.21`, with labels `app=web`.
2. Perform a rolling update to upgrade image from `nginx:1.21` to `nginx:1.23`.
3. Roll back Deployment to previous version using `kubectl rollout undo`.
4. Scale the Deployment `web-deploy` to 5 replicas.
5. Add a `readinessProbe` to pause traffic during start.
6. Add a `livenessProbe` to auto-recover on failure.
7. Patch Deployment to update container environment variable without redeployment.
8. Pause rollout of Deployment and resume it later.
9. Observe `ReplicaSet` created under Deployment and inspect revision history.
10. Delete Deployment and verify ReplicaSet deletion behaviour.
11. Set maxSurge=1 and maxUnavailable=0 for controlled update.
12. Use Deployment strategy `Recreate` for stateful application.
13. Inject ConfigMap into Deployment containers via envFrom.
14. Inject Secret as volume in Deployment.
15. Mount a PVC into a Deployment container.
16. Set imagePullSecrets on Deployment.
17. Add annotations and labels to Deployment metadata.
18. Set resource requests and limits.
19. Override container command with entrypoint logic.
20. Create a Deployment with multiple containers.
21. Add initContainers in Deployment.
22. Simulate container crash and watch Deployment auto-recovery.
23. View Deployment status with `kubectl rollout status`.
24. Patch Deployment to use a new image tag.
25. Apply a Deployment using `kubectl apply -f` and observe the diff using `kubectl diff`.
