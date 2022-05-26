# socat_nc

Very very simple echo server set up

## Server

```
socat -v tcp-l:8000,fork exec:"/bin/cat"
```

## Client

### with socat

```
socat -v tcp-connect:localhost:8000 stdin
```

### with nc

```
nc localhost 8000
```

That's it. Easy.


