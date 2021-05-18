# Fess on Kubernetes

fessctl is an utitly to manage [Fess](https://fess.codelibs.org/) on Kubernetes.
fessctl creates Kubernetes cluster on [kind](https://kind.sigs.k8s.io/) as default.

## Usage

### Create Fess on Kubernetes

```
$ ./fessctl create -k kind
```

-k option is kubernetes type. You can spcify `kind` or `eks`.

### Use Proxy

```
$ ./fessctl proxy
```

### Use CUrl

```
$ ./fessctl curl https://localhost:9200
```

### Delete Fess on Kubernetes

```
$ ./fessctl delete -k kind
```

