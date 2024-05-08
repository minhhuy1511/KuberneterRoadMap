This is noted and tutorial of my roadmap in kubernetes.
Welcome

PART I - K8S

1. Into
2. What is Kubernetes (k8s)?
Vm bao gồm: Applib, node, OS/
Docker đóng gói container
Container: Đóng gói run time, os, app, lib
Orchestration: quản lý tổ chức containner ví dụ như K8s
3. Yes and No K8s
Popular (64% production)
Innovation - rapid change
Cost
Hiring People and long term development
Strong community
job oppoturnity
flexible and security
 
Not Recommend

Learning Curve
Complexity (Docker Swarm, Nomad, Amazone ECS)
4. K8s Archirect
Control Plan (Master Node)
    API-Server: Nhân thông tin từ scheduler để chuyển khai 
    Scheduler: Tính toán triền khai pod trên Worker node nào dựa trên ETCD
    ETCD: Cơ sở dữ liệu dạng key value
    Controller Manager: Giám sát baseline của cluster ổn định giáo tiếp API-server
    Cloud-Manager
    Container Runtime
Worker node (Data Plane)
    kubelet: nhận thông tin từ API_server để chuyển khai pod trên Work node
    Container Runtime
    Kube proxy: tướng tác với các pod và các ứng dụng mạng
5. k8s - Control Plane components
(https://kubernetes.io/releases/version-skew-policy/)
https://kubernetes.io/releases/patch-releases/#support-period
6. K8s - Worker Node components
7. Install Dockert and minikube

- Docker install: https://docs.docker.com/engine/install/ 
- Docker hub repos: https://hub.docker.com/repositories/v...
- Install kubectl: https://kubernetes.io/docs/tasks/tools/ 
- kind: https://kind.sigs.k8s.io/ 
- minikube installation: https://minikube.sigs.k8s.io/docs/start/ 
8. Imperative vs Declarative
9. Pod - Imperative
10. Pod - Declarative
11. NodePort Service
12. Service Types
13. Namespaces
14. Lables & Selectors
15. ReplicaSet
16. Deployments
17. Rolling Updates & Rollbacks
18. Taints & Tolerance
19. NodeSelector
20. NodeAffinity
21. Pod - Environment variables
22. ConfigMaps
23. Secrets
24. InitContainers
25. Liveness & Readiness Probes
26. Volumes
27. Persistent Volumes
28. Persistent Volumes Claims
29. Custer Networking
30. Service Networking 
