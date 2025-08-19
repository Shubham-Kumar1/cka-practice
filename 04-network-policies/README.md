## 4. **Network Policies**

1. Create a default deny-all ingress NetworkPolicy for namespace `dev`.
2. Allow ingress only from Pods with label `role=frontend` to app Pods.
3. Allow egress to external IP 8.8.8.8 on port 53 (DNS).
4. Allow traffic only on TCP port 80 from Pods in same namespace.
5. Create NetworkPolicy to allow ingress only from specific namespace.
6. Create a policy allowing egress to Pods labeled `db=true`.
7. Apply a policy to multiple Pod selectors.
8. Allow ingress traffic from `10.244.0.0/16` CIDR block.
9. Combine ingress and egress rules in one policy.
10. Allow ingress only on port 443.
11. Deny all egress except for TCP port 443.
12. Allow traffic from specific ServiceAccount.
13. Use `namespaceSelector` to restrict by labels.
14. Test policy with `busybox` client Pod.
15. Allow all egress traffic to internet (wildcard).
16. Allow ingress from specific Pod IPs.
17. Chain multiple policies for combined behavior.
18. Audit network traffic before applying policy.
19. Use `kubectl exec` to test reachability.
20. Use `netcat` to test open/closed ports.
21. Apply a policy and observe traffic drop using logs.
22. Use `networkPolicyPeer` with IPBlock.
23. Use `except` field to blacklist subnets.
24. Monitor network policies using `cilium monitor` (if using Cilium).
25. Validate enforcement of NetworkPolicy with e2e tests.