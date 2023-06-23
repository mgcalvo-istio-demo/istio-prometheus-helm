#
https://istio.io/latest/docs/setup/install/helm/

helm repo add istio https://istio-release.storage.googleapis.com/charts

helm search repo istio

NAME                               	CHART VERSION	APP VERSION	DESCRIPTION                                       
bitnami/wavefront-adapter-for-istio	2.0.6        	0.1.5      	DEPRECATED Wavefront Adapter for Istio is an ad...
istio/istiod                       	1.18.0       	1.18.0     	Helm chart for istio control plane                
istio/base                         	1.18.0       	1.18.0     	Helm chart for deploying Istio cluster resource...
istio/cni                          	1.18.0       	1.18.0     	Helm chart for istio-cni components               
istio/gateway                      	1.18.0       	1.18.0     	Helm chart for deploying Istio gateways           
istio/ztunnel                      	1.18.0       	1.18.0     	Helm chart for istio ztunnel components




kubectl create namespace istio-system

helm install istio-base istio/base -n istio-system --version 1.18.0
