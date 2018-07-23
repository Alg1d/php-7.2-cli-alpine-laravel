# PHP 7.2 CLI Docker definition

This is based on the [laradock Dockerfile](https://github.com/laradock/laradock/blob/master/php-worker/Dockerfile) but with the following changes:
 * removed all the optional features for speed
 * mcrypt php extension
 * mailparse php extension
 * includes composer so we can run composer install in Bitbucket pipelines
 * bash and mysql-client - so we can use the image in Bitbucket pipelines 

Available on Dockerhub here: [netfiradev/php-7.2-cli-alpine](https://hub.docker.com/r/netfiradev/php-7.2-cli-alpine/)  