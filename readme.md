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
Pod một đơn vị triền khai dịch vụ, 1 pod có thể gồm 1 hoặc nhiều container
10. Pod - Declarative
11. NodePort Service
Expose pod: nodeport, loadbalancer
NodePort: 30.000 -32.762
Vidu: 10.100.5.8:30198

kubectl get pods: Lấy các pods
kubectl describe pods app1: Mô tả pod
kubectl get service: lấy các service
Kubectl describe svc service1: Mô tả service
kubectl expose pod app1 --port=8081 --target-port = 8080 --name:service1 --type=NodePort: phơi pod ra ngoài internet thông qua nodeport
kubectl get nodes -o wide: xem thông tin của node với option wide
kubectl logs app1 -f : xem log tren pod co 1 container hien tai
kubectl logs app1 -c logs: xem logs trong pod co container logs
kubectl exec -it app1 --ls: truy cập vào container list folder
kubectl exec -it app1 --sh: ssh vào container
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
