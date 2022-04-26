![kenzo github stats](https://github-readme-stats.vercel.app/api?username=kenzok8&show_icons=true&theme=merko)
<div align="center">
<h1 align="center">自用稳定OpenWRT仓库——网络收集</h1>
</div>


#### djpackage

*  自用常用OpenWrt软件包源码合集，同步上游更新！

*  感谢github仓库所有创作者！

##### 关于Secrets、TOKEN的小知识


1. 首先需要获取 **Github Token**: [点击这里](https://github.com/settings/tokens/new) 获取,

 `Note`项填写一个名称,`Select scopes`不理解就**全部打勾**,操作完成后点击下方`Generate token`

2. 复制页面中生成的 **Token**,并保存到本地,**Token 只会显示一次!**

3. **Fork** 我的`small-package`仓库,然后进入你的`small-package`仓库进行之后的设置

4. 点击上方菜单中的`Settings`,依次点击`Secrets`-`New repository secret`

其中`Name`项填写`ACCESS_TOKEN`,然后将你的 **Token** 粘贴到`Value`项,完成后点击`Add secert`

* 对应`.github/workflows`目录下的`yml`工作流文件里的`ACCESS_TOKEN`名称（依据自己yml文件修改）

* 在仓库`Settings->Secrets`中添加 `SCKEY `可通过[Server酱](http://sc.ftqq.com) 推送编译结果到微信

* 在仓库`Settings->Secrets`中添加 `TELEGRAM_CHAT_ID, TELEGRAM_TOKEN `可推送编译结果到`Telegram Bot`


#### 使用方式（三选一）：

1. 先cd进package目录，然后执行

```bash
 git clone https://github.com/zikexiaozi/djpackages
```
2. 或者添加下面代码到feeds.conf.default文件

```bash
 src-git djpackages https://github.com/zikexiaozi/djpackages
```
