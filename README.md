# Organization Knowledge Graph Search Engine

This is a knowledge graph of organizations ready for search. The knowledge graph is built by 

* crawling data from open-source websites, and 
* using advanced NLP and knowledge extraction and alignment algorithms to transform the webpages to knowledge graph
* storing the knowledge in a Elasticsearch to allow the users to search the organizations by names

To use it: 

### 1. pull the docker from the docker hub

```bash
docker pull ruzeliang/organization_search:1.0.1
```

### 2. run the docker

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

<img src="service%20ready.png" width="600">




### 3. open the input interface of FLASK 

http://localhost:2644/

### 4. input the company name you want to search from the knowledge graph

<img src="input%20interface.png" width="500">


### 5. click "Excute" to search

<img src="search.png" width="600">

### 6. open the search result interface from 

http://localhost:5611/browser/

### 7. see the search results of the knowledge graph for the company "Upwork"

<img src="knowledge%20graph%20search%20result.png" width="800">
