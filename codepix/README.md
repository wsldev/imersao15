```bash
# acessar codepix container
docker exec -it codepix-app-1 bash
# executar proto
protoc --go_out=application/grpc/pb --go_opt=paths=source_relative --go-grpc_out=application/grpc/pb --go-grpc_opt=paths=source_relative --proto_path=application/grpc/protofiles application/grpc/protofiles/*.proto
```

````bash
kafka-topics --list --bootstrap-server=localhost:9092
kafka-console-consumer --topic=teste --bootstrap-server=localhost:9092
``