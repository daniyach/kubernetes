## Creación de manifiestos para kuberentes
- vamos por el deploymnet del template de aiprism, tenemos todos lo ficheros y la imagen docker.
- Tenemos el despliegue del pod con la imagen correctamente ahora queremos viisualizar ese pod utilziando ingress.


importante para utilizar una imagen docker que solo esta local debemos de seguir lo siguiente:

1. Set the environment variables with eval $(minikube docker-env)
2. Build the image with the Docker daemon of Minikube (e.g., docker build -t my-image .)
3. Set the image in the pod specification like the build tag (e.g., my-image)
4. Set the imagePullPolicy to Never, otherwise Kubernetes will try to download the image.

[stackOverflow](https://stackoverflow.com/questions/42564058/how-can-i-use-local-docker-images-with-minikube)
[Documentación kubernetes](https://kubernetes.io/docs/concepts/containers/images/#image-pull-policy)