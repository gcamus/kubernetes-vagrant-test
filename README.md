http://kubernetes.io/docs/getting-started-guides/kubeadm/

kubeadm init --pod-network-cidr=10.244.0.0/16 --api-advertise-addresses=http://192.168.56.101
kubectl taint nodes --all dedicated-
kubectl apply -f https://raw.githubusercontent.com/coreos/flannel/master/Documentation/kube-flannel.yml



kubeadm join --token=0cd317.8fca773365c1b01f 192.168.56.101