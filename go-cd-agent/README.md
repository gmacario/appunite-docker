# Go CD Agent

## Building

```bash
docker build --tag appunite/go-cd-agent:latest .
```

## Running

```bash
docker run -e GO_SERVER=ci.appunite.net -d --name go-cd-agent appunite/go-cd-agent:latest 
```

## TTY

```bash
docker run \
      -e GO_SERVER=ci.appunite.net \
			--tty -i \
			appunite/go-cd-agent:14.4.0 /bin/bash
```			
