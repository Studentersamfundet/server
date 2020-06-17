# Putting a nginx vhost into service mode

This can be put in a location block to restrict access to a certain ip address. It is recommended to restrict access to 127.0.0.1/localhost and do SSH port forwarding to get access.
```
if ($remote_addr != "127.0.01") {
    return 503;
}
```
