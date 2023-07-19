# KubeBuilder Example

[![Open in DevPod!](https://devpod.sh/assets/open-in-devpod.svg)](https://devpod.sh/open#https://github.com/loft-sh/devpod-kubebuilder-guestbook)

## Quickstart 

Either click on the 'Open in DevPod' link above or start via `devpod up github.com/loft-sh/devpod-kubebuilder-example`. This will start a small devcontainer that has all the needed tools to start working on a custom Kubernetes controller. It will also start a small KinD cluster within the devcontainer that can be used for development.

After successfully starting the devcontainer, you can then start the project via:

```
make install && make run
```

Then install the example Guestbook CRD into the cluster:

```
kubectl apply -f config/samples/webapp_v1_guestbook.yaml
```

Now you can view it via:

```
kubectl get guestbooks
```

Congrats, you just completed the kubebuilder quickstart. For further information, please take a look at their [official docs](https://book.kubebuilder.io/quick-start.html#test-it-out).
