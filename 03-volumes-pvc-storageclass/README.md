# 03-volumes-pvc-storageclass

## ✅ 3. **Volumes, PVCs, Storage Classes**

1. Create a `PersistentVolume` (PV) of 1Gi storage backed by `hostPath` at `/data/pv1`.
2. Create a `PersistentVolumeClaim` (PVC) of 1Gi storage using `ReadWriteOnce` access mode.
3. Create a Pod that uses a PVC to mount data at `/mnt/data`.
4. Create a StorageClass with `reclaimPolicy: Retain`.
5. Bind a PVC using a dynamically provisioned StorageClass.
6. Delete a PVC and inspect if PV is retained.
7. Reuse a released PV by resetting its claimRef.
8. Create a StorageClass using `volumeBindingMode: WaitForFirstConsumer`.
9. Create a PVC that is `Pending` and troubleshoot the issue.
10. Use `nfs` backed PV and mount in a Pod.
11. Create multiple PVCs and mount them in one Pod.
12. Create Pod with ephemeral inline volume using `emptyDir`.
13. Use `subPath` in volumeMount to map only sub-directory.
14. Resize a PVC by updating its spec.
15. Verify volume expansion status.
16. Delete a PVC and recreate Pod to observe behavior.
17. Use `volumeMounts.readOnly: true` for read-only access.
18. Create a Pod with a CSI volume using a supported plugin.
19. Test `hostPath` vs `emptyDir` behaviors.
20. Configure Pod to use `projected` volume combining ConfigMap, Secret.
21. Mount volume with `mountPropagation`.
22. Use `secret` volume to inject TLS certificate.
23. Backup volume data using `kubectl cp` or `initContainer`.
24. Set `storageClassName: ""` in PVC to bind manually.
25. Mount same PVC in multiple Pods (RWO vs RWX scenarios).