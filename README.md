Clair With Wait
===============

A Docker image and compose file for running CoreOS's
[Clair](https://github.com/coreos/clair) service. The only difference with the
official image at quay.io/coreos/clair is that this adds
[wait-for-it.sh](https://github.com/vishnubob/wait-for-it) which
makes it easy to wait for the postgres service to become available.

A better fix would be to add a wait with backoff to the Go code as per Kelsey
Hightower's [12 fractured
apps](https://medium.com/@kelseyhightower/12-fractured-apps-1080c73d481c#.f0x9bkj1j). Until then, you may find this useful.

Adrian.
