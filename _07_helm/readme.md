install helm by the docks of the helm website

helm create apache-helm
helm package apache-helm 
helm install dev-apache apache-helm -n dev-apache --create-namespace
helm uninstall dev-apache
helm rollback dev-apache 2 -n dev-apache 
