
1. Start EFK

```
$ docker-compose up
```

2. Start test service

```
$ docker-compose -f web-docker-compose.yml up
```

3. poke test service

```
$ repease 10 curl http://localhost:8080/
```

4. Go to http://localhost:5601/ -> Discover, and set first pattern `fluentd-*`, then click next step.

5. OK, you can search the logs!
