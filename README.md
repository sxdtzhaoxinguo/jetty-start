# jetty-start
jetty start web project!

# jetty-start 项目说明 #

该项目是用来通过jetty启动web项目的，直接引入该依赖就行，当前版本为：1.0.1-SNAPSHOT

# 使用案例 #
1.在项目中的pom.xml中引入该依赖
<dependency>
	<groupId>com.micai.jetty.start</groupId>
	<artifactId>jetty-start</artifactId>
	<version>1.0.1-SNAPSHOT</version>
</dependency>

2.编写启动项目的类：
package com.yingjun.ssm;

import com.micai.jetty.start.JettyServerStart;

public class BeautyStart {

	public static void main(String[] args) throws Exception {
		String webapp = "src/main/webapp";
        new JettyServerStart(webapp, 8080, "/").start();
    }
	
}

3.默认访问路径：http://localhost:8080
