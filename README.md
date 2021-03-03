# dwebssh

Run SSH over [dSwarm](https://github.com/dwebprotocol/dswarm)!

```
npm install -g dwebssh
```

On a server or some laptop with ssh-server running run

```sh
dwebssh-server
```

This will print out the ssh fingerprint and start announcing the server
on the dWeb network under this fingerprint.

To connect to the server on another computer simply pass in the fingerprint
and the user you want to connect as to dwebssh

```sh
dwebssh ssh-ed25519 AAAA.... maf
```

That's it! No more remembering hostnames :D

In addition this forwards the ssh fingerprint to the client so your connection cannot be
man-in-the-middle'd.

Does UDP hole punching through dSwarm so it's great for making your office server available over ssh
even if that server is behind a firewall

## License

MIT
