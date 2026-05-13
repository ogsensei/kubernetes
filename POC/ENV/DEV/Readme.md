Istio
helm install base /home/og/istio/base -f base.yaml -n istio-system
helm install istiod /home/og/istio/istiod -f istiod.yaml -n istio-system
helm install cni /home/og/istio/cni -f cni.yaml -n istio-system

Istio Ingress
helm install gateway /home/og/istio/gateway -f gateway.yaml -n istio-system

Istio kilai

Argo
helm install argocd /home/og/istio/argo-cd -f argocd.yaml -n argocd