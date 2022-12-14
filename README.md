## Build an Image ##

```docker build --tag test_955 .```

## Run an image ##

```docker run --name con_955 -p 8090:8080 test_955```

## If you are using windows operating system try to run the below command before running the CURL commands ##

```Remove-item alias:curl```

## Run the curl command ##

This transfers ETH:

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"0xb41243470b3f379fbFe652d69c742207336A7A5e\",\"amount\":\"0.05\"}' http://localhost:8090/eth```
                                                                            
This transfers token:

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"0xb41243470b3f379fbFe652d69c742207336A7A5e\"}' http://localhost:8090/token```
































<!-- docker-compose up -->
<!-- ## Build an Image ##

```docker build --tag nci02 .```


## Run an image ##

```docker run --name ncilab02 -p 8090:8080 nci02```

## Run the curl command ##

This transfers ETH:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0xac4FafdA6A3A6B48b4cDC2a896acf8D104C81d6C", "amount":"0.05"}' http://localhost:8090/eth```

This transfers token:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0xac4FafdA6A3A6B48b4cDC2a896acf8D104C81d6C"}' http://localhost:8090/token``` -->

