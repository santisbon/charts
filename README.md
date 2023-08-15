# Helm charts

These are published on Artifact Hub. To search:
```shell
helm search hub [KEYWORD] --list-repo-url --max-col-width [uint] -o [table|json|yaml]
```
For example:
```shell
helm search hub pi-hole --max-col-width 70 --list-repo-url
```
To add this repo and install one of its charts:
```shell
helm repo add santisbon https://santisbon.github.io/charts/

helm install $RELEASE $CHART --version $VERSION -n $NAMESPACE
# or directly from https://santisbon.github.io/charts/<.tgz file>
```

More details:  
* [Pi-hole](https://github.com/santisbon/pi-hole-k8s)  
* [speedtest](https://github.com/santisbon/speedtest)  