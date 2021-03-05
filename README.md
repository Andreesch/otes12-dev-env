# otes12-dev-env
Repositório para fornecer instruções de como configurar um ambiente de desenvolvimento local para as aulas de OTES-12 (tópicos avançados em engenharia de software)  utilizando Java e Spring Boot.

# Preparando seu ambiente de desenvolvimento

## Sistema Operacional Linux 

- Para utilizar esse componente, basta seguir esses passos:

1) Abra o seu terminal do linux utilizando o atalho CTRL + SHIFT + T;

2) Execute o comando abaixo:

```
sudo apt install openjdk-11-jre
```

3) Verifique se o Java foi instalado corretamente na sua máquina digitando o comando abaixo no terminal

```
java --version

```
O output desse comando deverá ser:

```
openjdk 11.0.10 2021-01-19
OpenJDK Runtime Environment 18.9 (build 11.0.10+9)
OpenJDK 64-Bit Server VM 18.9 (build 11.0.10+9, mixed mode)
```

4) Instale o maven utilizando o comando abaixo:

```
sudo apt update
sudo apt install maven

```

5) Verifique se a instalação do maven foi executada com sucesso

```
mvn -version
```

O output desse comando deverá ser:

```
Apache Maven 3.6.3
Maven home: /usr/share/maven
Java version: 11.0.10, vendor: Oracle Corporation, runtime: /home/andrecristofolinischneider/.sdkman/candidates/java/11.0.10-open
Default locale: pt_BR, platform encoding: UTF-8
OS name: "linux", version: "5.8.0-44-generic", arch: "amd64", family: "unix"
```

### Usando o demo

Dentro da pasta raiz do repositório, existe uma pasta com o nome "demo" onde você poderá encontrar um projeto criado para utilizar este componente usando o framework Spring Boot.

- Para utilizar esse projeto, basta seguir esses passos:

1) Gerar o arquivo .jar do projeto, que é possível navegando até a pasta raiz e executando o comando abaixo:

```
mvn clean package install
```

2) Rodar o arquivo .jar do projeto

```
mvn spring-boot:run
```

3) Acessar a URL do swagger (OPCIONAL)

```
http://localhost:5000/swagger-ui.html
```

### Endpoints


#### Calcular Estadia

``POST http://localhost:5000/api/v1/stay``

Calculo de uma estadia.

* nights: Quantidade de noites.
* costPerNight: Custo por noite.
* guestExpensesList: Despesas do hospede.

JSON de criação:
`{
  "costPerNight": 125,
  "guestExpensesList": [
    4.50,66
  ],
  "nights": 2
}`

JSON de resposta:
`{
  "paymentValue": 336.53
}`
