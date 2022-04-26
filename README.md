## 1、初始化
```bash
cnpm i
# 我用npm i 未能初始胡成功
```
## 2、部署说明
修改文件
#### (1)、邮箱配置
```js
// config\config.default.js
// 邮箱配置
		email: {
			client: {
			host: 'smtp.qq.com',
			secureConnection: true,
			port: 465,
			auth: {
				user: '************@qq.com', // QQ 邮箱
				pass: '************' // QQ密钥
			}
			}
		}
```
#### (2)、数据库配置
```js
// MongoDB数据库配置
        mongoose:{
            client: {
                url: 'mongodb://127.0.0.1:27217/cloudNew', // user是collection(数据库)名称
                options: {
                    useUnifiedTopology: true
                },  // 其他配置项
            }
        },
```
## 3、匹配Elecon客户端
https://github.com/cgq001/e-api-electron