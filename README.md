# Fess on Kubernetes

fessctl is an utitly to manage [Fess](https://fess.codelibs.org/) on Kubernetes.
fessctl creates Kubernetes cluster on [kind](https://kind.sigs.k8s.io/) as default.

## Usage

### Create Fess on Kubernetes

```
$ ./fessctl create -k kind
```

-k option is kubernetes type. You can spcify `kind` or `eks`.

### Proxy Access

#### Elasticsearch

Run a proxy as below:

```
$ ./fessctl proxy -t elasticsearch
```

and then

```
$ ./fessctl curl https://localhost:9200
```


#### Fess

Run a proxy as below:

```
$ ./fessctl proxy
```

and then

```
$ curl https://localhost:8080
```

### Delete Fess on Kubernetes

```
$ ./fessctl delete -k kind
```

