# git-module-test

使用git submodule命令为git仓库添加子模块，每个子模块都是一个独立的git项目 
eg： git submodule add git@github.com:Castlebin/python-learn.git python-learn

添加后，可以看到目录下多了一个.gitmodules文件，里面记录了git子模块的仓库地址等信息


    # cat .gitmodules

    [submodule "python-learn"]
            path = python-learn
            url = git@github.com:Castlebin/python-learn.git
    [submodule "config-server"]
            path = config-server
            url = git@github.com:spring-cloud-samples/configserver.git
    [submodule "turbine"]
            path = turbine
            url = git@github.com:spring-cloud-samples/turbine.git
    [submodule "zuul-server"]
            path = zuul-server
            url = git@github.com:spring-cloud-samples/zuul-server.git

## 完整的git子模块使用说明：
https://git-scm.com/book/zh/v1/Git-%E5%B7%A5%E5%85%B7-%E5%AD%90%E6%A8%A1%E5%9D%97
