# go_web_03
Web application in golang with revel framework.

## 1. Setup
```bash
$  git config --global http.sslVerify true
$  go get -u github.com/revel/cmd/revel
$  revel new go_web_03
~
~ revel! http://revel.github.io
~
Your application is ready:
   /Users/502662077/Documents/workspace_go/src/go_web_03

You can run it with:
   revel run go_web_03

$  revel run go_web_03
```

Go to `http://localhost:9000/` and you'll see:

    "It works"

Move it to the correct location:
```bash
$ mv go_web_03 github.com/rwibawa/
SFO1502662077M:src 502662077$ cd github.com/rwibawa/go_web_03
SFO1502662077M:go_web_03 502662077$ revel run
```

## 2. Code Layout

The directory structure of a generated Revel application:

    conf/             Configuration directory
        app.conf      Main app configuration file
        routes        Routes definition file

    app/              App sources
        init.go       Interceptor registration
        controllers/  App controllers go here
        views/        Templates directory

    messages/         Message files

    public/           Public static assets
        css/          CSS files
        js/           Javascript files
        images/       Image files

    tests/            Test suites


## 3. Help

* The [Getting Started with Revel](http://revel.github.io/tutorial/gettingstarted.html).
* The [Revel guides](http://revel.github.io/manual/index.html).
* The [Revel sample apps](http://revel.github.io/examples/index.html).
* The [API documentation](https://godoc.org/github.com/revel/revel).

## 4. govendor
```bash
  $  go get -u github.com/kardianos/govendor
  $  govendor init
  $  govendor add +external
  $  govendor list
```
