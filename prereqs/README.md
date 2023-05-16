1. install OpenShift GitOps Operator
2. oc apply -f prereqs/sealed-secrets/application.yml -n openshift-gitops
3. generate sealed secret from htpasswd and kubernetes secret at sealed secrets web
4. oc apply -f prereqs/app-project.yml