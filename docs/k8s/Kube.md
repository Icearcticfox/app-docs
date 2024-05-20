
**Debug busybox**
kubectl run curl-my --image=radial/busyboxplus:curl -i --tty --rm
**Real-time logs**

kubectl logs -f -l app=duty-slack-app --max-log-requests 11   -n miniweb-testing
kubectl logs --since=6h -l app=reporter -n miniweb-b
kubectl edit roles.rbac.authorization.k8s.io leader-election-role
Kubetail oauth2-proxy -n Grafana-system
kubectl apply --force -f test_volume.yaml -n grafana-test

**Helm**
helm template tempo-vulture/chart -f tempo-vulture/chart/values.yaml > file.yaml
helm template test helm -f cronjobs/.merged_values.yaml > file.yaml
helm create mychart
helm template my-release mychart
helm get all ingress-nginx -n miniweb-system --revision 4 > miniweb-test-ingress-nginx-4.yaml

**k8s criteo repo**

**generate config**

rm -fr build/ && python3 setup.py build && python3 setup.py install
  
**deploy**

k8s-conf-cli deploy --env preprod --data-centers da1 --kube-clusters kubes99 observability/tempo
  
**list release**

k8s-conf-cli list-apps