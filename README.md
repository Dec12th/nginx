## 1.本地创建编译完成之后， Nginx 最终目录

```
sudo mkdir /apps
chmod 777 /apps
```

## 2.下载代码到用户目录

```
cd ~
mkdir github && cd github
git clone git@github.com:lightningMan/nginx.git
```

## 3.配置、编译、安装

```
cd ~/github/nginx
run
```

## 4.验证编译是否成功

### a.编译完之后的 Nginx 所有的文件可以在 `/apps/nginx` 中找到，你可以通过以下指令来验证

```
cd /apps/nginx/sbin
nginx
```
然后，打开你的浏览器，输入 http://127.0.0.1 便可看到效果

### b.由于本仓库编译出来的代码是可以集成到 clion 中 debug 的，因此，你必须确保 `~/github/nginx/objs` 下有名为 `nginx` 的文件，并且此文件也可以直接运行

```
cd ~/github/nginx/objs
nginx
```

## 集成到 clion

我们的目标当然是直接修改源码，并且最终按一下 Debug，就自动完成编译，运行，效果如下



![集成 clion](http://g.recordit.co/buhZFdFnAE.gif)





那么到底如何实现？且听下回分解。









