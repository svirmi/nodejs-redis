##### Docker Compose with multiple local containers
##### node.js (React) + redis

##### To build image run
```bash
docker build -f Dockerfile.dev .
```

##### Just to run built container use
```bash
docker run -it -p 3000:3000 <CONTAINERID fcafb0470bac>
```

##### App is running at http://localhost:3000/

##### To run tests inside a container:
```bash
docker run -it <CONTAINERID fcafb0470bac> yarn test
```

##### Running container with volumes mapping and live code chagging detection:
```bash
docker run --rm -it -p 3000:3000 -v /app/node_modules -v $(pwd):/app 18403a4bf0dd
```
