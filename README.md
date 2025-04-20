# ☸️ kubectl — CLI for Kubernetes

**kubectl** is the command-line tool for interacting with Kubernetes clusters. It allows you to deploy applications, inspect and manage cluster resources, and view logs and events.

---

## ✅ Features

- Manage and inspect Kubernetes clusters
- Deploy applications and updates
- Monitor pods, services, deployments
- Execute commands inside containers
- View logs, events, and cluster status

---

## 🔧 Installation

### Debian/Ubuntu
```bash
sudo apt update
sudo apt install -y kubectl
```

### Arch Linux
```bash
sudo pacman -S kubectl
```

### macOS (Homebrew)
```bash
brew install kubectl
```

### Verify installation
```bash
kubectl version --client
```

---

## 🚀 Basic Usage

### Check cluster info
```bash
kubectl cluster-info
```

### List all pods
```bash
kubectl get pods
```

### List services
```bash
kubectl get svc
```

### Deploy from YAML
```bash
kubectl apply -f deployment.yaml
```

### Describe a pod
```bash
kubectl describe pod <pod-name>
```

### Delete a pod
```bash
kubectl delete pod <pod-name>
```

---

## ⚙️ Common Commands

| Command                                   | Description                              |
|------------------------------------------|------------------------------------------|
| `kubectl get nodes`                      | Show all cluster nodes                   |
| `kubectl get all`                        | Show all resources in current namespace  |
| `kubectl logs <pod>`                     | Show logs from a pod                     |
| `kubectl exec -it <pod> -- bash`         | Access pod shell                         |
| `kubectl port-forward <pod> 8080:80`     | Forward port to a pod                    |
| `kubectl delete -f file.yaml`            | Delete resources defined in YAML         |

---

## 🧩 Tips

- Organize your configs in a `manifests/` folder for easy management.
- Use `kubectx` and `kubens` for fast context and namespace switching.
- Combine `watch` for real-time monitoring:
  ```bash
  watch kubectl get pods
  ```

---

## 📚 More Info

- Docs: [https://kubernetes.io/docs](https://kubernetes.io/docs)  
- GitHub: [https://github.com/kubernetes/kubernetes](https://github.com/kubernetes/kubernetes)  
- Run `kubectl --help` or `man kubectl` for all commands
