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
