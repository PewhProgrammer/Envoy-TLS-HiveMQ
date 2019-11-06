FROM envoyproxy/envoy:latest

ADD ./certs/example-com.crt /etc/example-com.crt
ADD ./certs/example-com.key /etc/example-com.key

# RUN apt-get update && apt-get -q install -y \
#    curl

CMD /usr/local/bin/envoy -c /etc/front-envoy.yaml --service-cluster front-proxy    
