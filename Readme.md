# provision-servers

Minimal server provisioning with shell scripts via SSH.

## Features

* Allows you to use tools that you already have to bootstrap your servers.

## Anti-Features

* Does not require learning a complicated DSL.
* Does not attempt to be clever about the operating system's package manager.
* Does not attempt to be clever about idempotency (most of the time, idempotency is free in linux anyway).
* Does not require you to pre-setup a provisioning server or pay someone to do it for you.

## Example

    % ssh <HOSTNAME> '$SHELL' < ubuntu/ci-jenkins

NOTE: To cheaply try this, spin up a DigitalOcean droplet (or equivalent) and replace `<HOSTNAME>` in the command above.

## Resources

- [10 advanced, yet digestible SSH techniques][techniques]

## Alternatives

* [puppet]
* [chef]
* [ansible]

## License

MIT

[puppet]:     http://puppetlabs.com
[chef]:       http://www.getchef.com/chef
[ansible]:    http://www.ansibleworks.com
[techniques]: https://speakerdeck.com/wilmoore/10-advanced-yet-digestible-ssh-techniques

