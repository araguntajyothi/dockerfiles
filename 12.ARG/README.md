### ARG

 * ARG is used to supply few variables at the time of image creation

 * ENV is useful at the time of both image creation and container creation, but arg it is only useful at the time of image creation

 * Till now we have seen that FROM should be the first instruction for dockerfile. but there is a exception  to this rule. If we want to use ARG in our dockerfile then FROM should be the second

 * Sometimes we may want to use different version of  the same package in our dockerfile. For example, we may want to use python 3.
 *  We can use ARG to supply the version of python at the time of image creation. We can use
 *  ARG in the following way:

```
   ARG PY_VERSION
   FROM python:${PY_VERSION}
```
* so build image using below command:

```

docker build -t araguntajyothi/arg:v1 --build-arg PY_VERSION=3.9 .
```

* ARG is the only instruction you can use before FROM. ARG Declared before from cannot access after from.
* But ARG declared after from can be accessed.

### Using ENV and ARG for best results.
 * Create one env variable and assign the value of ARG to that env variable.
 * Then we can access ARG values through ENV both in image and container.


