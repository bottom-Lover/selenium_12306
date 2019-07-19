# selenium_12306
本项目是python3 + selenium实现在12306官网自动订票的

主要参考：hack12306项目 https://github.com/xiaoshun007/12306Python

下载与运行之前需知：
（1）安装依赖包：
  pip install splinter,configparser
（2）下载chromedriver驱动：
  参考 https://chromedriver.storage.googleapis.com/index.html 此界面下载（注意下载的版本与你使用的版本保持一致）

下载与运行：直接clone到本地，在selenium目录下运行py test.py即可。（注意在运行之前更改配置文件，配置文件中有详细说明，请在运行之前仔细阅读并更改）

与hack12306的区别：
（1）hack12306是用Python3 + splinter写的，有些底层的东西没法实现，例如无法使用WebDriverWait方法等待元素加载完毕；
（2）hack12306有些bug未修复，作者发现的在此项目中都已作出修改。

运行时：
  运行之后谷歌浏览器会自动打开，并会自动填充用户名和密码（运行之前必须在配置文件填写用户名和密码），填充完毕后等待用户点击验证码，验证完成之后会帮你自动订票，直至订票完成。（其中若有什么bug，请加我微信联系或者在GitHub中留言，谢谢！）
