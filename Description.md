### IMAGES
use `keversc/php-deployer:5` to deploy php5 applications

use `keversc/php-deployer:7` to deploy php7 applications

### USAGE
`docker run -it -v $PWD:/app keversc/php-deployer:7 deploy stage`

If you an authentication method that require an external file (i.e. `identityFile()` that require `~/.ssh/id_rsa.pub` for example), you must add a volume:

`docker run -it -v $PWD:/app -v ~/.ssh:/root/.ssh keversc/php-deployer:7 deploy vp` 