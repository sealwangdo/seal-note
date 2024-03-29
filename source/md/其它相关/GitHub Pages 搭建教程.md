# GitHub Pages 搭建教程



著作权归 Brick713 所有。 链接：https://sspai.com/post/54608



互联网从诞生发展至今日，每天有无数的人在上面留下自己的足迹，他们用它记录生活、抒发情感、分享见解，这一切都离不开一个可以承载文字的平台，一个独立的、由自己掌控的平台，而 GitHub Pages 就是这么一个平台。

在这个平台里你可以使用自己的个性域名；可以在海量的主题里挑选最适合你的那一款，如果你技术极客，也可以根据自己的喜好，设计属于自己的个性化页面；你既可以在线创建和发布网站，也可以在本地通过客户端工具或者命令行进行网站和内容的管理。

你完全可以通过 GitHub Pages 展示和输出自身价值，甚至可以把它打造成属于自己的互联网「身份证」。

## 为什么使用 GitHub Pages

如果你把他作为一个轻量级的个人博客服务，GitHub Pages 相较 WordPress 之类的建站服务有什么优势呢？

- 首先他是完全免费的，相较其他的同类产品，他能替你省下一笔服务费，节约下的钱可以让你买一些其他的会员服务；
- 无须自己购买云服务进行搭建，只需按步骤一步步操作即可，即使你不懂他的技术细节；
- 支持的功能多，玩法丰富，你可以绑定你的域名、使用免费的 HTTPS、自己 DIY 网站的主题、使用他人开发好的插件等等；
- 当完成搭建后，你只需要专注于文章创作就可以了，其他诸如环境搭建、系统维护、文件存储的事情一概不用操心，都由 GitHub 处理

当然了，作为一款免费的服务，我们也是要遵守 GitHub 官方使用建议和限制，在使用的时候项目和网站的大小不要超过 1GB，也不要过于频繁的更新网站的内容（每小时不超过 10 个版本），每个月的也要注意带宽使用上限为 100GB。

综合来看，GitHub Pages 依旧可以说是中小型博客或项目主页的最佳选项之一。

## 如何使用 GitHub pages

介绍了这么多，下面就具体来谈谈如何使用它。

### 基本页面的生成

首先你需要注册一个 GitHub 账号，并在个人主界面里选择创建一个新的 Repository 。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2vpuv8j20v40943zm.jpg)

进入页面后，在 Repository name 的位置填写域名，格式是 `username.GitHub.io`。

创建成功之后，点击右上角的 Settings

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2w7rjij20v408gdgw.jpg)

找到 GitHub Pages 选项，选择一个 GitHub 官方提供的主题

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2nsvexj20v4021t8m.jpg)

这里我们就随意选择一个主题 Cayman，来看看他的效果是什么样的

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2xmpupj20v40ek0ty.jpg)

选择完毕之后 GitHub Pages 就会自动帮你生成好网站，在他跳转的界面点击 Commit changes 按钮，网站就可以访问了。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2ygjxfg21lu0u0jvr.gif)

在浏览器里输入你的项目名称，比如 [brick713.GitHub.io](https://brick713.github.io/)，就可以看到，你刚刚选择的主题的个人网站的页面了。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2x6t0vj20u00w5q5f.jpg)

到这里如果你只是想做一个例如可以随时在互联网上访问的简历，那么你只需要 GitHub Pages 项目的主页修改你 [index.md](http://index.md/) 文件就可以了，比如我给出的这个模板。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2prfj0j20u0118go6.jpg)

修改完后，点击上图中左下角的 Commit Changes，然后访问你的自定义域名你就可以看到如下的样式了。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2ocp2bj20u01csjtr.jpg)

如果你想做一个功能更丰富的博客，那我们继续往下走。

### 配置自定义域名并免费使用 HTTPS

在 2018 年 5 月 1 日之后，GitHub Pages 已经开始提供免费为自定义域名开启 HTTPS 的功能，并且大大简化了操作的流程，现在用户已经不再需要自己提供证书，只需要将自己的域名使用 CNAME 的方式指向自己的 GitHub Pages 域名即可。

首先在你的 DNS 解析里添加一条解析记录，例如我选择添加子域名 `blog.moyu.life` 通过 CNAME 的方式指向我刚刚自定义的 GitHub Pages 域名 `brick713.GitHub.io`。添加完成后等待 DNS 解析的生效（DNS 的解析记录生效到全球可能需要几分钟时间）。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2nnyo7j20v40emabf.jpg)

之后重新回到最开始进入过的 Settings 界面，找到 GitHub Pages 的设置，填写我们刚刚建立的子域名，以我自己的 blog.moyu.life 举例，点击保存。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2vb2uaj20v40pg0vi.jpg)

保存后 GitHub 需要一定的时间生成证书并确认域名的解析是否正常，我们只需要耐心的等待即可，成功后显示结果如下

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2she52j20v40pan04.jpg)

现在我们再访问 blog.moyu.life 就会发现，我们的自定义域名和 HTTPS 都生效了！可以看到证书是由著名的机构 Let's Encrypt 提供的。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2v02e5j20v40hujt4.jpg)

### 网站的同步

现在我们已经有了一个基本功能健全的网站了，接下来我们需要试着对博客的内容进行管理，并且给博客添加一些更个性化的设置，官方提供两种方式：

- 命令行方式（Mac 和 Windows 确保拥有 Git 环境）
- 桌面客户端形式（需要安装官方提供的客户端）

如果你没有任何 Git 的基础，也不想进行一些繁琐的配置，那么我推荐你使用桌面客户端的形式进行管理，如果你有一定的技术基础，那么 Git 的方式则更适合你。这里我两种方法都介绍一下。

首先在命令行中切换到你自定义的路径下，然后 Clone 下来你的项目（操作需要在 Mac 的 Terminal 中完成，Windows 系统可以使用 Git-bash。）这里注意这里的 path 和 username 需要根据你个人情况进行替换。

```
cd ~/Path git clone https://GitHub.com/username/username.GitHub.io
```

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2tekiaj20v407zjsi.jpg)

接着进入你的项目的文件中，并创作一个文章。

```
cd username.GitHub.io
echo "Hello World 我爱这个世界" > index.md
```

然后按照 Git 提交内容的流程，将我们的新创作的文章上传。

```
git add --all
git commit -m "Firs Push"
git push -u origin master
```

这里可能会碰到下面的情况：

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2swmu0j20v40cnjsi.jpg)

按照他的提示我们把注册 GitHub 的邮箱和用户名依次输入即可：

```
git config user.email "你的邮箱"
git config user.name "你的用户名"
```

之后他可能会让你输入你的 GitHub 账号和密码，不用担心，正常输入即可。当我们看到这样的提升就证明提交成功了。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2ryrf3j20sc0aggn2.jpg)

可以去我们的网站主页看看是不是起了变化。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2os5a6j20v40gygm2.jpg)

如果你是使用[GitHub 桌面客户端](https://desktop.github.com/) 那么就更简单了，下载安装了客户端之后，按照客户端的提示正常登陆你的 GitHub 账号。然后 Clone 下来你的 GitHub Pages 项目。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2qmgsrj20v40lejt9.jpg)

等待 Clone 完成后，界面上会显示几种管理修改你的项目的方式。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2rmpogj20v40le765.jpg)

这里我选择使用 Sublime Text 进行管理，把开始的 [index.md](http://index.md/) 里的内容改为 `Hello World 我也爱这个世界` 保存，然后在客户端上我们能看到文件的变化，我们先点击左下角的 Commit to master，再点击 Fetch origin 就可以将内容上传。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2ud354j20v40lcwfm.jpg)

然后你发现你的主页也发生了相应改变了。到这里你基本上就掌握了网站管理的基本流程和文章发布的基本流程，下面我们要开始来学会使用静态模板系统来管理博客了。

### GitHub Pages 的生成工具

经历了上面的步骤，现在你的已经有了一个简单的页面了，可是他还远远未满足我们的需求，我们需要利用静态模板系统来让生产接管你博客的文章的生成，让你把更多的经历投入在创作里。下面就 GitHub 官方推荐的 Jekyll 为例子来展开讲讲。

因为 Jekyll 是基于 Ruby 的静态网页生成系统，因此我们首先得安装 Ruby 环境，在 Mac 下我们可以使用的 Homebrew 来进行安装。如果是其他操作系统，可以去参考 [Ruby 官方安装文档](https://www.ruby-lang.org/en/documentation/installation/)进行安装。

```
brew install ruby
```

等 Ruby 安装完毕后再执行以下命令完成 Jekyll 的安装。

```
gem install jekyll bundler
```

然后进入你 Clone 下来的 GitHub Pages 项目的路径，例如：

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2q4wx1j20pc04cgm0.jpg)

执行以下命令：

```
jekyll new . --force
```

完成后，Jekyll 会在你指定的目录下生成好所有文件，你可以使用 `bundle exec jekyll serve` 命令，然后就可以通过访问 `127.0.0.1:4000` 查看初始界面的样子了。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2r2t80j20v40ohmyb.jpg)

默认的界面看起来非常的简陋也很丑，但是没关系，你可以在这些网站里根据自己的喜好找到一些美观的主题http://jekyllthemes.org/、https://jekyllthemes.io/、http://themes.jekyllrc.org/。

安装方法很简单，一般情况下只需要下载主题包解压后完整的，复制到你的 GitHub Pages 的项目目录里，并覆盖你之前的文件即可，有些特殊的主题要参考作者给的安装步骤，这里我随意的更换了一个主题。

![img](https://tva1.sinaimg.cn/large/e6c9d24egy1h2ds2wrky3j20u00xojtk.jpg)

主题里的所有关键性配置都在 _config.yml 文件中，你可以根据个人的喜好和不同主题支持的功能来修改具体的内容，这里就不做展开。

到这里完整的搭建的流程已经结束了，你已经可以正常访问你一路配置下来的博客了，接下来你只需要找一个趁手的 Markdown 编辑器来编辑在你本地 GitHub Pages 项目中的 _posts 文件夹里的文章，并使用前面提到的两种方式将文章同步到 GitHub 上即可。需要注意的是，文章的内容和标题需要按照 Jekyll 的格式进行写作。

文章的文件名遵循下面的格式：

```
年-月-日-标题.markdown
```

文章内容顶部必须有下面的 YAML 头信息：

```
---
layout: post
title: Blogging Like a Hacker
---
```

## 尾巴

其实除了 Jekyll 还有非常多的第三方的静态模板系统来搭建 GitHub Pages。比如：

- Node.js 编写的 Hexo
- Go 编写的 Hugo
- Python 编写的 Pelican
- 以及更人性化的 Gridea

他们在各自的基础上实现了更多的功能，比如分析统计、搜索、评论系统、广告、分享系统等。喜欢折腾的同学不妨可以尝试尝试，未来如果有机会希望能更详细的给大家分享一下。