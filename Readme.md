### Recap

Please refer this [repo](https://github.com/madhank93/learn-k8s-ckad) to go through the core concepts of k8s.

### Q&A

1. <details>
   <summary> What need to be installed in Control plane and Worker node ?</summary>

   <p>

   ![ctr-wrk-node](assets/img/cp-wrk-node.png)

   **Control plane** - API server, Scheduler, ETCD and Controller manager, Kubelet, Kube proxy and Container runtime

   **Worker node** - Kubelet, Kube proxy and Container runtime

   </p>
   </details>

1. <details>
   <summary> What are Static pods ?</summary>

   <p>

   Static Pods or Master pods (API server, Scheduler, ETCD and Controller manager) are managed directly by the kubelet daemon on a specific node, without the API server observing them or control plane. `Kubelet` continuously watches for `/etc/kubernetes/manifests` folder on a node and schedules the pods according to the manifests files.

   For more info refer [here](https://kubernetes.io/docs/tasks/configure-pod-container/static-pod/)

   </p>
   </details>
