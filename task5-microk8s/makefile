install-microk8s:
	sudo snap install microk8s --classic

enable-addons:
	sudo microk8s enable dns dashboard

status:
	sudo microk8s status --wait-ready

deploy-nginx:
	sudo microk8s kubectl apply -f nginx-deployment.yaml

expose-nginx:
	sudo microk8s kubectl apply -f nginx-service.yaml

serve-nginx-locally:
	sudo microk8s kubectl port-forward service/nginx-service 8070:80

