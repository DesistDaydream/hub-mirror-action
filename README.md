# Github 代码同步 Gitee
同 https://github.com/Yikun/hub-mirror-action
该项目逻辑：通过 github action 功能，触发流水线。通过 Dockerfile 构建镜像，通过通过 entrypoint.sh 脚本将 github 上的仓库逐一同步到 gitee 上。
所以只有一个 workflows 目录下的 action 配置文件不够。

参考[这里](https://blog.csdn.net/sculpta/article/details/104897320)可以通过在每个项目里配置单独 target 来为每个项目配置同步功能，这里就不用构建 docker 之类的了。