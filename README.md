# grafana

Charts and configurations 

### Run
```

docker run -it --rm --user 104 \
    -v=${PWD}/grafana/grafana.ini:/etc/grafana/grafana.ini \
    -v=${PWD}/grafana/data:/var/lib/grafana \
    -v=${PWD}/grafana/provisioning:/etc/grafana/provisioning \
    -p 3000:3000 grafana/grafana

docker run -d --restart always --name=grafana \
    -v=${PWD}/grafana/grafana.ini:/etc/grafana/grafana.ini \
    -v=${PWD}/grafana/data:/var/lib/grafana \
    -v=${PWD}/grafana/provisioning:/etc/grafana/provisioning \
    -p 3000:3000 grafana/grafana
    
```
