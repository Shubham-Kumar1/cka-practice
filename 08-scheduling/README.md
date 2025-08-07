# 08-scheduling

## ✅ 8. **Scheduling**

1. Use `nodeSelector` to schedule Pod on node with label `tier=backend`.
2. Use `affinity` to ensure two Pods co-schedule on same node.
3. Use `antiAffinity` to distribute Pods across nodes.
4. Use `preferredDuringScheduling` to give soft preference.
5. Taint a node and schedule Pod with matching toleration.
6. Prevent Pod from scheduling using unsatisfiable affinity.
7. Configure `podTopologySpreadConstraints`.
8. Manually drain a node and reschedule Pods.
9. Create a custom Scheduler and assign Pods.
10. Use `nodeName` to bind Pod directly to a node.
11. Schedule a critical Pod with `priorityClassName`.
12. Create a custom PriorityClass with high value.
13. Observe preemption of low-priority Pods.
14. Reserve CPU using `resource requests`.
15. Schedule Pod with `resource limits` only.
16. Validate eviction due to node pressure.
17. Bind Pod manually using `kubectl bind` (deprecated).
18. Simulate scheduler stuck on unsatisfiable Pod.
19. Use `schedulerName` to assign Pod to custom scheduler.
20. Simulate inter-Pod affinity with custom labels.
21. Avoid node with `NoExecute` taint.
22. Create taint-tolerant workloads.
23. Use `kubectl cordon` and observe effects.
24. Create large Podset and observe binpacking.
25. Debug Pending Pod due to scheduling failure.