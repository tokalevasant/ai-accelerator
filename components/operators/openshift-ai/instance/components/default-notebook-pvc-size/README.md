# default-notebook-pvc-size

## Purpose
This component is designed help admins configure the default PVC size that users are presented with when creating new Workbenches.

## Usage

This component can be added to a base by adding the `components` section to your overlay `kustomization.yaml` file:

```
apiVersion: kustomize.config.k8s.io/v1beta1
kind: Kustomization

resources:
  - ../../base

components:
  - ../../components/default-notebook-pvc-size
```

You can customize the pvc size by updating the [patch-rhoai-dashboard.yaml](./patch-rhoai-dashboard.yaml) file.