# ai-vision   
# ai-vision    
## 定位   
日常生活和学习用到的辅助工具，主要应用于办公和文本编辑。    
## 现有功能描述   
- 手写体识别   
- 中英互译   
## 待开发功能   
- 读取Excel格式图片并将图片中的文字导入Excel中   
- 读取PDF格式图片，在对应位置输出含图片和文字的word文档   
- 图片内容识别   
- 图片中人物表情识别   
## 现有应用实现流程   
### ocr识别应用   
- 1.注册讯飞开放平台账号
- 2.免费试用手写体服务
- 3.记录该服务对应的识别码
- 4.在微信公众平台的开发者服务中填入ocr识别的服务器域名
- 5.下载该服务的nodejs例子
- 6.wx.request替换request-promise请求
- 7.将识别到的内容展示到xml中
- 8.添加复制、全选和个别选择的功能
### 中英互译
同上操作，需要改变的只有服务类型
### 历史记录查询
- 1.在app.js中写死数据库集合
- 2.在应用中添加数据库的增操作
- 3.在用户也根据用户的openid进行数据库查询操作，并将数据分条展示
- 4.调用长按监听方法进行数据库的删除操作
## 使用三方工具
- 引入接口 讯飞开发平台
- 数据存取 小程序云服务中的数据库和CDN存储
- 调用工具类 crypto-js 
