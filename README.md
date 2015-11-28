# zhihu-collection
知乎离线收藏夹

## 简介
  能够帮你抓取知乎中的收藏夹, 专栏, 回答. 收藏夹和专栏可以整体抓取, 也可以抓取单独的收藏夹和专栏文章, 单独的答案抓取会被归类到名人堂专栏
	使用Express + Mongodb + Node.js

## 使用
	1. 启动mongodb
	2. 调用lib的接口进行抓取, 抓取的结果会保存在mongodb中, 具体例子可以看app.js
	3. node worker.js 启动服务器进程, 通过http://localhost:3000 进行浏览

## 注意
	由于知乎有些收藏夹需要登录才能浏览, 你可以在lib/uitl.js中设置Cookie, 然后进行抓取, 默认是没有设置Cookie的


## Done
- [x] 模仿Node.js API 布局
- [x] 调整答案图片大小
- [x] 添加作者链接
- [x] 答案点击跳转
- [x] 选中链接加下划线
- [x] 加入专栏分栏, 收缩列表
- [x] 返回顶部按钮
- [x] 测试收藏夹一个问题, 有多个答案的情况
    - 除了第一个答案, 之后没有标题
- [x] 防止答案删除功能
- [x] 获取编辑时间 
- [x] 抓取分页
- [x] 名人堂分栏



## Todo
- [ ] 关键字搜索
- [ ] 服务器自动刷新最新文件情况
- [ ] 输入url抓取指定的收藏夹
- [ ] 设置定时抓取任务

## License
MIT
