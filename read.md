# Springcloud 项目整合

# spring cloud Eureka

* 常用的api

API说明	| URL	| 请求方式
查询所有的应用实例	http://localhost:8761/eureka/apps	GET
根据AppId查询应用实例	http://localhost:8761/eureka/apps/{app}	GET
根据 AppId 及 instanceId 查询	http://localhost:8761/eureka/apps/{app}/{instanceId}	GET
根据 instanceId 查询	http://localhost:8761/eureka/instances/{instanceId}	GET 
注销应用实例	http://localhost:8761/eureka/apps/{app}/{instanceId}	DELETE
注册新应用实例	http://localhost:8761/eureka/apps/{app}	POST
暂停/下线应用实例	http://localhost:8761/eureka/apps/{app}/{instanceId}/status?value=OUT_OF_SERVICE 	PUT
恢复应用实例	http://localhost:8761/eureka/apps/{app}/{instanceId}/status?value=UP	PUT
应用实例发送心跳	http://localhost:8761/eureka/apps/{app}/{instanceId}	PUT 
修改应用实例元数据	http://localhost:8761/eureka/apps/{app}/{instanceId}/metadata?version=1.0.1	PUT