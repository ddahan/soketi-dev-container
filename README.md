# Soketi Dev Container

### URLs

* https://github.com/soketi/soketi


### Run

* Create config file from example
* Run `soketi start --config=config_<env>.json`

### Todos

* Not 12 factors compliant for now. Use env file instead as soon as we use for production.

### Warning

* If the provided app id contains non-digit chars, the pusher libs can not connect to it. See [this issue](https://github.com/soketi/soketi/issues/491).
