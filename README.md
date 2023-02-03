# kubernetes-manifests-devops

This repo contains all the manifests to deploy automatically the services we add on top on k3s from a devops perspective.
This is highly recommended to use ansible to deploy these manifests automatically.

## How to use

This is highly recommended to use ansible to deploy these manifests automatically.

### Apply

Once the k3s cluster setup and deployed, it should be automatically deployed if you use ansible. However, if you decide to deploy it manually, just set the local variable KUBECONFIG toi point on the kubeconfig file retrieved for the k3s cluster and run `kubectl apply -f ./`.

### Delete

To delete all the devops deployments, just run `kubectl delete -f ./`.