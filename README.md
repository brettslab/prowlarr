# Prowlarr

Prowlarr is deployed through the `overlays` Kustomize overlay.

## Network

The production overlay exposes Prowlarr through MetalLB:

```text
http://192.168.50.212:9696
```

## Storage

The base creates a `prowlarr-config` PVC using the `ceph-rbd` StorageClass.
