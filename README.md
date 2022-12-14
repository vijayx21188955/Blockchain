## Build an Image ##

```docker build --tag test_955 .```

## Run an image ##

```docker run --name con_955 -p 8090:8080 test_955```

## If you are using windows operating system try to run the below command before running the CURL commands ##

```Remove-item alias:curl```

## Run the curl command ##

This transfers ETH:

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"Destination Address\",\"amount\":\"Desired Amount\"}' http://localhost:8090/eth```
                                                                            
This transfers token:

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"Destination Address\"}' http://localhost:8090/token```


