# react-reverse-proxy

```
minikube start mount $DIR:$DIR

cd nginx

minikube image build -t nginx-reverse-proxy .

cd ..

minikube image build -t react .

cd kubetemplates/

kubectl apply -f .

kubectl port-forward service/nginx 8080:80
```
