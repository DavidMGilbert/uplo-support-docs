# Using Uplo on a remote node

## Using Uplo on a remote node

While the majority of users use Uplo on a local computer, there are a few instances where it is either not possible or more useful to run a Uplo node on a remote server.

Uplo already has the functionality to automatically pick up a running `uplod` instance if one was started manually. To get Uplo to pick up a remote instance, all you need to do is forward your local port 9980 to your remote server port 9980. For those comfortable with the command line, you can use the following command.

```text
ssh -f user@domain -L 8480:localhost:8480 -N
```

`-f` Requests ssh to go to background just before command execution.

`-L` Specifies that the given port on the local \(client\) host is to be forwarded to the given host and port on the remote side.

`-N` Do not execute a remote command.

Now when you restart Uplo, it will pick up the remote instance of uplod. All API calls that don't require authentication will work, however API calls that require authentication will fail as the UI will be using the wrong API password. A workaround for this is to restart the remote uplod instance with:

`--authenticate-api=false`

Now, all API calls will work and you can use Uplo just like you would with a local uplod instance.

