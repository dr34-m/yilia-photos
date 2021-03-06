# yilia-photos
yilia的相册
这是[Litten](http://litten.me/)相册的修改版，版权归原作者所有

#### [点此预览效果](https://blog.ctftools.com/photos/)

### 使用说明

#### 本相册适用于hexo-yilia主题，移植到其他主题需要改动

#### 与原作者相比改动
1.由原作者图片托管在instagram改为托管在本地

2.由原作者图片尺寸固定改为尺寸可以写入ins.json

3.去掉原作者type选项，只可以放图片而不能放视频，并且图片格式只支持jpg（如果需要支持更多格式对ins.js稍作修改即可）

4.link作为图片名

5.去掉ins.jsn中的src选项

### 使用方法

1.将本项目所有文件保存到您hexo的source目录下的一个目录里

2.在本目录新建ins与minins文件夹，将原图片保存到ins文件夹下，图片略缩图保存在minins文件夹下，略缩图推荐尺寸:328x328

3.之后source目录树一般如下
```
├── _posts
├── photos
|   ├── ins
|   |   ├──pic1.jpg
|   |   ├──pic2.jpg
|   |   └──pic3.jpg
|   ├── minins
|   |   ├──pic1.min.jpg
|   |   ├──pic2.min.jpg
|   |   └──pic3.min.jpg
|   ├── index.ejs
|   ├── ins.css
|   ├── ins.js
|   └── ins.json
└── CNAME
```

4.如果原图名称为xxxx.jpg，则略缩图名称为xxxx.min.jpg

5.修改ins.json与您实际情况相匹配，其中图片名不需要写后缀，描述部分随意，图片尺寸格式为图片宽度x图片高度，例如：
```
{
	"date": "2015-05",
	"arr": {
		"year": 2015,
		"month": 5,
		"link": ["201505251818"],
		"text": ["这是一张在2015年五月拍摄的照片"],
		"sizes": ["1000x1000"]
	}
}
```
照片太多可以自己写程序简化操作，可以看下我曾用过的思路[https://blog.ctftools.com/2017/12/post234/](https://blog.ctftools.com/2017/12/post234/)

略缩图可下载这个软件批量生成

链接: [https://pan.baidu.com/s/1slULnUd](https://pan.baidu.com/s/1slULnUd) 密码: 54je
