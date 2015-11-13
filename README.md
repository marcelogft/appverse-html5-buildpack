# appverse-html5-build
Appverse HTML5 Build Dockerfile

[![dockeri.co](http://dockeri.co/marcelogft/appverse-html5-buildpack/)](https://registry.hub.docker.com/marcelogft/appverse-html5-buildpack/)

* NodeJS 
* Bower
* Grunt (grunt-cli)


Usage

Create a Dockerfile in your nodejs application directory with the following content:

```
FROM mcolomer/appverse-html5-build

WORKDIR /myapp
ADD . /myapp
RUN npm install && bower install

EXPOSE 9000

CMD ["grunt", "server"]
```
