# GitHub 上面的HowTo Index
## 微服务
* 本机启动基础设施快速指引
  * Prometheus: https://github.com/ryanzhang/quarkus-quickstart/tree/master/metrics-quickstart#%E5%90%AF%E5%8A%A8prometheus
  * Grafana: https://github.com/ryanzhang/quarkus-workshop-labs#run-grafana 
  * Jaeger: https://github.com/ryanzhang/quarkus-quickstart/tree/master/metrics-quickstart#opentracing-using-jaeger
  * Kafka: https://github.com/ryanzhang/quarkus-quickstart/tree/master/kafka-quickstart#%E5%90%AF%E5%8A%A8kafka
    * docker compose: https://github.com/ryanzhang/quarkus-quickstart/blob/master/kafka-quickstart/docker-compose.yml
  * Artimis: https://github.com/ryanzhang/quarkus-quickstart/tree/master/amqp-quickstart#%E5%90%AF%E5%8A%A8-artimis
  * Infinispan: https://infinispan.org/blog/2019/12/02/image/ (infinispan必须用sudo启动)
  * postgresql:
      podman run --name postgres -e POSTGRES_USER=postgres \
                                 -e POSTGRES_PASSWORD=postgres -e POSTGRES_DB=my_data \
                                 -p 5432:5432 postgres:10.5
                     or
      podman run --ulimit memlock=-1:-1 -it --rm=true --memory-swappiness=0 \
           --name postgres-quarkus-hibernate -e POSTGRES_USER=hibernate \
           -e POSTGRES_PASSWORD=hibernate -e POSTGRES_DB=hibernate_db \
           -p 5432:5432 postgres:10.5
  * Keycloak:  
   * 容器启动: 
   * 非容器启动以及配置： https://raw.githubusercontent.com/ryanzhang/springboot-restful-crud/msa-ss-sso/keycloak/run.sh?token=AAEAVKN6NEZC2FAV3DTZBNS6VP32Q
  * wildfly: https://github.com/ryanzhang/simple-war#deploy-example-assuming-in-linux-terminal
  * redis https://github.com/ryanzhang/github-housekeep#redis
  
##
* 命令行启动spring contract: https://github.com/ryanzhang/coolstore/tree/master/catalog#how-to-start-contract-by-stub-runner-command-line

## 常用的SaaS api服务
 * Star war 人物: https://swapi.dev
 * github api https://github.com/ryanzhang/github-housekeep#github-api
 
## 加速
 * 国内镜像加速: https://gist.github.com/y0ngb1n/7e8f16af3242c7815e7ca2f0833d3ea6
  

