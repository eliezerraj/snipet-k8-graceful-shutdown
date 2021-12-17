# snipet-k8-graceful-shutdown

1. create a namespace 
kubectl apply -f deployment-namespace.yaml

2. create a deployment
kubectl apply -f deployment.yaml

3. Make deployment
kubectl replace -f deployment.yaml

4. Check logs
kubectl logs -f pod/go-graceful-shutdown-8484d6ffc7-cx9ck -n test-c

5. Check rollout update
kubectl rollout status deployment go-graceful-shutdown -n test-c

