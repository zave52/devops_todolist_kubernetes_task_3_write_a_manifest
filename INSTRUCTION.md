# Instruction of applying all kubernetes manifests

## Applying manifests

### 1. Create namespace

```bash
kubectl apply -f .infrastructure/namespace.yml
```

### 2. Create busybox pod

```bash
kubectl apply -f .infrastructure/busybox.yml
```

### 3. Create todoapp pod

```bash
kubectl apply -f .infrastructure/todoapp-pod.yml
```
