# organization_knowledge_graph_search

### pull the docker from the docker hub

```bash
docker pull ruzeliang/organization_search:1.0.1
```

### run the docker

```bash
docker run -it ^
-p 0.0.0.0:9344:9344 ^
-p 0.0.0.0:3641:3641 ^
-p 0.0.0.0:5611:5611 ^
-p 0.0.0.0:4971:4971 ^
-p 0.0.0.0:2644:9000 ^
ruzeliang/organization_search:1.0.1
```
