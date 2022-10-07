# k8s Playground

## Load testing with Fortio

Run the following command to load test the application
```
kubectl run -it fortio --rm --image=fortio/fortio -- load -qps 2000 -t 220s -c 70 "http://goserver-service/healthz"
```