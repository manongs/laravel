# laravel 教程
经常有人问我，PHP有没有好用的框架，我说laravel框架啊，国际php大咖专业、全职的做这个框架，不二的选择啊。
> laravel 5.5是官方新发布的版本，是一个长期支持版本，所以建议大家学习5.5,下面简单说明一下不同版本之间的差别
  * 一般发行版 - 只提供 6 个月的 Bug 修复支持，一年的安全修复支持。
  * LTS 版本 - 长期支持版本，英文 Long Term Support 的缩写，此类版本是 Laravel 能提供的最长时间维护版本,例如 Laravel 5.1，提供两年的错误修复和三年的安全修复。
## 目录
- [简介](#简介)
- [运行要求](#运行要求)
- [环境安装](#环境安装)
- [Composer安装](#Composer安装)
- [Laravel安装](#Laravel安装)

## 简介
> Laravel这个名字来自于纳尼亚传奇中的Cair Paravel城堡，在故事中国王和皇后居住其中。Laravel 和Paravel 的发音相似，Taylor认为Laravel这个名字韵味深长而又优雅，所以命名为Laravel。Cair Paravel 中的Paravel发音为['pærəvel]  推断Laravel发音取['lærəvel]
  
## 运行要求
> 但如果你不使用 Homestead，则需要确保你的服务器符合以下要求
  * PHP >= 7.0.0
  * PHP OpenSSL 扩展
  * PHP PDO 扩展
  * PHP Mbstring 扩展
  * PHP Tokenizer 扩展
  * PHP XML 扩展
 
## 环境安装
  请大家下载的时候，一定要下载php7以上的版本，最好下载php7.1以上的版本
  * [Homestead](https://d.laravel-china.org/docs/5.5/homestead)
  > 虚拟机环境(支laravel功能最全的环境，也是较为难装的环境，主要是vagrant的镜像是国外的，下载非常慢，建议用VPN错开高峰时下载)
  * [XAMPP](https://www.apachefriends.org/zh_cn/download.html)
  > 集成开发环境，支持windows,mac
  * [MAMP & MAMP PRO](https://www.mamp.info/en/downloads/)
  > 集成开发环境，支持mac,windows

## Composer安装
  Composer是什么？请进入这个传送门[Composer](http://www.phpcomposer.com/)

## Laravel安装
  * 通过 Laravel 安装器
  ```php
  //全局安装laravel安装器
  composer global require "laravel/installer"
  //通过laravel安装器安装laravel
  laravel new demo
  ```
  * 通过Composer安装(如果执行了上一步，请跳过这一步)
  ```php
    composer create-project --prefer-dist laravel/laravel demo
  ```
  * laravel配置
  ```php
  //拷贝配置文件
  cp .env.example .env
  ```
  * 运行实例
  ```php
  php artisan serve
  ```
  用浏览器打开：[http://127.0.0.1:8000](http://127.0.0.1:8000),此命令使用了php内置服务器打开，在没有数据库参入的时候，可以使用，如果涉及到复杂应用，请在开发环境中打开对应的url
