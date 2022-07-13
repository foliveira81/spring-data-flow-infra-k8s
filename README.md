# spring-data-flow-infra

kubectl create -f /spring-cloud-dataflow/src/kubernetes/mysql/
kubectl create -f /spring-data-flow-infra/prometheus/prometheus-clusterroles.yaml
kubectl create -f /spring-data-flow-infra/prometheus/prometheus-clusterrolebinding.yaml
kubectl create -f /spring-data-flow-infra/prometheus/prometheus-serviceaccount.yaml

kubectl create -f /spring-data-flow-infra/prometheus/prometheus-proxy/
kubectl create -f /spring-data-flow-infra/prometheus/prometheus-configmap.yaml
kubectl create -f /spring-data-flow-infra/prometheus/prometheus-deployment.yaml
kubectl create -f /spring-data-flow-infra/prometheus/prometheus-service.yaml
kubectl create -f /spring-data-flow-infra/grafana/
kubectl create -f /spring-data-flow-infra/prometheus-proxy/

kubectl create -f /spring-data-flow-infra/server/server-roles.yaml
kubectl create -f /spring-data-flow-infra/server/server-rolebinding.yaml
kubectl create -f /spring-data-flow-infra/server/service-account.yaml
kubectl create -f /spring-data-flow-infra/skipper/skipper-config-rabbit.yaml
kubectl create -f /spring-data-flow-infra/skipper/skipper-deployment.yaml
kubectl create -f /spring-data-flow-infra/skipper/skipper-svc.yaml
kubectl create -f /spring-data-flow-infra/server/server-config.yaml
kubectl create -f /spring-data-flow-infra/server/server-svc.yaml