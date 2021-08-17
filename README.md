# terratest-example

Iniciando o test a partir do link [https://terratest.gruntwork.io/docs/getting-started/quick-start/](https://terratest.gruntwork.io/docs/getting-started/quick-start/).

```sh
➜  go version
go version go1.16.5 linux/amd64
➜  terratest-example git:(main) ✗ terraform --version
Terraform v0.12.31

Your version of Terraform is out of date! The latest version
is 1.0.4. You can update by downloading from https://www.terraform.io/downloads.html
```

```sh
mkdir {examples,test}
touch examples/main.tf
touch test/example_test.go

cd test
go mod init "github.com/afonsoaugusto/terratest-example"
go mod tidy

go test -v -timeout 30m
```
