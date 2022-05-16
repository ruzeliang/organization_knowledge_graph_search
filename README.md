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

the docker will start the service of the knowledge graph for search, wait for a few minutes, until you see the following

![Alt text](service%20ready.png)



### open the input interface of FLASK 

http://localhost:2644/

### input the company name you want to search from the knowledge graph

![Alt text](input%20interface.png)

### click "Excute" to search

![Alt text](search.png)

