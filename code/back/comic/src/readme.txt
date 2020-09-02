新建业务模块在openplat包下
                                                                      需要配置jvm运行参数config.url为配置中心地址,profile为服务概要
                                                                      需要改动build.gradle文件中的group 'com.h3c.dzkf.web-template' 为所对应的group名称
                                                                      需要改动logback.xml <property name="LOG_HOME" value="${home}/logs/template/${profile}"/> 中的template为application-name
                                                                      需要改动build.gradle文件中的group 'com.h3c.dzkf.microservices.custom.ms-web-template' 将ms-web-template改为之前改动的服务名称
                                                                      需要改动setting.gradle文件中的名称为当前项目名称
                                                                      需要改动bootstrap.properties文件中的spring.application.name为当前服务名称
                                                                      需要改动bootstrap.properties文件中的spring.profiles.active(dev为测试环境,proc为生成环境)