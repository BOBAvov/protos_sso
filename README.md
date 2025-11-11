# protos
## Требуется для кодогенерации из proto файла
1. protoc
2. protoc-gen-go
3. protoc-gen-go-grpc
## Кодогенерация :
Удали старые файлы:
1. rm -r gen/go/sso/*
Сгенерировать новые
2. protoc -I proto proto/sso/sso.proto --go_out=./gen/go --go_opt=paths=source_relative --go-grpc_out=./gen/go/ --go-grpc_opt=paths=source_relative
