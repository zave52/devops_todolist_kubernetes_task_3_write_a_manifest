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


## Testing todoapp using port-forwarding

### 1. Verify that pods are running and ready

```bash
kubectl get pods -n todoapp
```

### 2. Apply port-forwarding

```bash
 kubectl port-forward pod/todoapp 8000:8000 -n todoapp
```

### 2. Open browser at [http://localhos:8000](http://localhos:8000) address
