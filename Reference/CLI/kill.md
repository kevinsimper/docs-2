## kill

    Usage: hyper kill [OPTIONS] CONTAINER

    Kill a running container

                --help               Print usage

The main process inside the container will be sent `SIGKILL`.

> **Note:**
> `ENTRYPOINT` and `CMD` in the *shell* form run as a subcommand of `/bin/sh -c`,
> which does not pass signals. This means that the executable is not the container’s PID 1
> and does not receive Unix signals.
