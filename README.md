
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



ref:

1. https://docs.docker.com/compose/install/#install-compose
2. https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html
3. https://www.elastic.co/guide/en/kibana/current/docker.html
4. https://www.jianshu.com/p/04f4d7b4a1d3
