## 前言

欢迎来到本项目的 Gitee 仓库！这是一个基于 Java 的原创歌曲分享平台毕业设计项目。在这里，我们将为你提供项目的完整源码、文档报告以及代码讲解，助你更好地理解和学习本项目的实现过程。

## 内容介绍

本项目是一款集歌曲分享、评论、点赞等功能于一体的原创歌曲分享平台。用户可以在平台上发布自己的原创歌曲，与其他用户互动，共同推动我国音乐创作事业的发展。此外，本项目还提供了丰富的后台管理功能，方便管理员对用户、歌曲、评论等内容进行管理。

## 技术介绍

- **语言**：Java
- **使用框架**：Spring Boot
- **前端技术**：JS、Vue、CSS3
- **开发工具**：IDEA/Eclipse
- **数据库**：MySQL 5.7/8.0
- **数据库管理工具**：phpstudy/Navicat
- **JDK版本**：jdk1.8
- **Maven**：apache-maven 3.8.1-bin
- **前端环境**：Node.Js 12\14\16

## 核心代码

以下是一段关于用户登录的核心代码：

```java
@PostMapping("/login")
public String login(@RequestParam String username, @RequestParam String password, HttpSession session) {
    User user = userService.findByUsernameAndPassword(username, password);
    if (user != null) {
        session.setAttribute("user", user);
        return "redirect:/";
    } else {
        return "login";
    }
}
```

这段代码定义了一个登录接口，用户输入用户名和密码后，系统会调用 `userService` 的 `findByUsernameAndPassword` 方法查询用户信息。如果查询成功，将用户信息存入 session，并跳转到首页；否则，返回登录页面。

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img14.360buyimg.com/ddimg/jfs/t1/312737/30/26722/106315/689ee9daF076650d6/e9529ab3fe633e15.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/314214/39/26553/20998/689ee9b6Fd2576129/ec67461f5433c378.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/315796/14/26456/56450/689ee9b6Fa7ec21e5/6f6b1a0bc1a3a3ca.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/318977/2/25343/13166/689ee9baF1a682186/a1acb189ba8032d6.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/302671/30/26082/16598/689ee9beF48e3ee18/4c6e48a6469d1f5f.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/324867/25/4775/73146/689ee9c5Fd65fed0d/0bed05a883a228b0.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
