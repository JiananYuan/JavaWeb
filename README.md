# JavaWeb简易笔记

### Servlet生命周期

init -> service -> destory -> 回收

![](https://www.runoob.com/wp-content/uploads/2014/07/Servlet-LifeCycle.jpg)

### 来自客户端的Http请求

```java
Enumeration it = req.getHeaderNames();
        while (it.hasMoreElements()) {
            String paramName = (String) it.nextElement();
            out.print("<tr><td>" + paramName + "</td>");
            String paramValue = req.getHeader(paramName);
            out.println("<td> " + paramValue + "</td></tr>\n");
        }
```

![0W319s.png](https://s1.ax1x.com/2020/10/12/0W319s.png)

### 来自服务器的Http响应

与Http请求的使用流程差不多：`PrintWriter out = resp.getWriter();`

### 来自服务器的响应状态码

- public void setStatus ( int statusCode )

- public void sendRedirect(String url)

- public void sendError(int code, String message)

### Section 会话

Servlet 提供了 HttpSession 接口，该接口提供了一种跨多个页面请求或访问网站时识别用户以及存储有关用户信息的方式。

Servlet 容器使用这个接口来创建一个 HTTP 客户端和 HTTP 服务器之间的 session 会话。会话持续一个指定的时间段，跨多个连接或页面请求。
















