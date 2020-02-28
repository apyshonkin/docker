Easy transparent proxy w/o cache or logging.

Create password file with htpasswd (apache2-utils) and place it wherever you want.

Then run it:

```docker run --name squid-lite -d -p 31289:31289 -v $PASSWORDFILE:/etc/squid/.squidusers:ro apyshonkin/squid-lite:1.0```

And now you can configure your device to external ip of your server and port 31289.
