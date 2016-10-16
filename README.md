### IMAGES
- `7`, `latest` [Dockerfile](https://github.com/kevin-verschaeve/php-deployer/blob/master/php7/Dockerfile)
- `5` [Dockerfile](https://github.com/kevin-verschaeve/php-deployer/blob/master/php5/Dockerfile)

### USAGE
`docker run -it -v $PWD:/app keversc/php-deployer:7 deploy stage`

If you choose an authentication method that require an external file (i.e. `identityFile()` that require `~/.ssh/id_rsa.pub` for example), you must add a volume:

`docker run -it -v $PWD:/app -v ~/.ssh:/root/.ssh keversc/php-deployer deploy stage` 