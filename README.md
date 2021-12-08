# HandsOn Confluent

## Criar um diretório especial de apps

Execute o comando:

```shell
mkdir -p ~/Apps/
cd ~/Apps/
```

## Baixar o pacote do Confluent 7.0.0

Execute o comando:

```shell
wget https://packages.confluent.io/archive/7.0/confluent-7.0.0.tar.gz
```

## Descompactar o pacote

Execute o comando:

```shell
tar -xvf confluent-7.0.0.tar.gz
```

## Incluir variáveis de ambiente em .zshrc (ou .bashrc)

Execute o comando:

```shell
code ~/.zshrc
```

ou 

```shell
code ~/.bashrc
```

Adicionar o seguinte conteúdo:

```shell
# CONFLUENT LOCAL-MACHINE
export CONFLUENT_HOME=~/Apps/confluent-7.0.0
export PATH=$PATH:$CONFLUENT_HOME/bin
```

## Recarregar variáveis de ambiente

Execute o comando:

```shell
source ~/.zshrc
```

## Teste Confluent Local

Execute o comando:

```shell
confluent --help
```


## Iniciar Confluent Local

Execute o comando:

```shell
confluent local services start
```

## Parae Confluent Local

Execute o comando:

```shell
confluent local services stop
```

## Analisar Log Confluent Local

Execute o comando:

```shell
confluent local services connect log
```

## Desmontar Confluent Local

Execute o comando:

```shell
confluent local destroy
```

## Acessar Control Center do Confluent Local

[http://127.0.0.1:9021/](http://127.0.0.1:9021/)