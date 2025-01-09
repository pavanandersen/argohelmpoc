# ELK Stack Helm Chart

Este Helm Chart implanta a stack ELK (Elasticsearch, Logstash, Kibana) no Kubernetes.

## Como usar

1. Clone este repositório:

git clone <url-do-repositorio>


2. Instale o Helm Chart:
helm install elk-stack ./elk-stack


3. Para verificar os serviços:
kubectl get all


4. Acesse o Kibana:
- Redirecione a porta local:
  ```
  kubectl port-forward service/kibana 5601:5601
  ```
- Abra no navegador: `http://localhost:5601`.

## Parâmetros

- O arquivo `values.yaml` permite personalizar os recursos e configurações de cada componente.
