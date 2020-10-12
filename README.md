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
















