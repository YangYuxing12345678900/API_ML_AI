# 智能便签APP

| 发布 | 2019年12月 |
|:----:|:----|
| 产品 | 智能便签app |
| 项目状态 | 完成 |
| 负责人 | 杨玉杏 |
| 设计师 | 杨玉杏 |
| 开发 | 杨玉杏 |
| 测试 | 杨玉杏 |


## 目标
快速将语音转文字记录需要的笔记，手写文字实现笔记电子化储存，可支持简单的文本翻译，方便人们的办公与学习

## 加值宣言 
本产品至于通过运用相关的人工智能价值，使用户在办公学习记录时达到更加便捷和使用的效果。运用**语音识别api**。摆脱按键操作，通过语音识别直接输入文字，方便笔记记录；同时可根据句意自动纠错、自动断句添加标点，保证文本输入的准确性。**手写文字识别api**，实现对手写文字、读书笔记、课堂笔记等内容的识别，实现对手写文字内容的电子存储；同时，实现对活动签到表、信息登记表、数据统计表等纸质表单内手写文字的识别，满足对纸质表单内信息进行统计整理、数据计算的需求，为办公学习记录保存数据提供更多样的方法。**通用翻译api**，语言翻译，在急需了解外语语义和转述中文时，提供一个更方便简要的内容翻译途径

## 核心价值 
本产品最小可行做到语音信息的快速转换文字信息记录，方便用户在不方便的情况下，快速记录要点信息；手写信息转写与通用翻译为辅助。改产品的宗旨在，让用户能在不方便的短时间内，实现便捷的信息记录。

## 核心价值与用户痛点 
* 痛点一：用户在记录信息要点和待办事项时，因忙于其他事物无法快速笔记或打字记录
* 痛点二：用户在用笔记记录信息或手绘表格后，需要转录电子版而需要花长时间的重新打字编辑和绘制
* 通电三：用户需要快速理解某句外文，而不能及时找到相应的工具；或在需要翻译语言给他人理解时

## 人工智能概率性与用户痛点 
* 百度语音识别api：存在进场中文普通话识别准确率达98%，同时支持普通话和略带口音的中文识别、个别方言粤语四川话识别和英文识别。
* 百度手写文字识别api：存在识别准确率可达90%以上，支持对图片中的手写中文、手写数字进行检测和识别，且对不断对不规则的手写字体进行识别专项优化
* Azure文本翻译api：通过 Translator API 的开放 REST 接口对超过 60 种支持语言的文本进行互译，轻松准确地检测任何文本字符串的语言，以决定需翻译哪个文本且翻译成哪种语言，但翻译结果的准确率没有绝对保障

各项人工智能的相应使用，并不能保证绝对的准确性。语音识别与手写文字识别的正确率高，但是还是会出现细小的错误。当语速过快或语调不正确，会出现识别差错；另外不同的人书写风格不同，过于潦草的字体可能会识别成其他自行相同的自。同时，通用翻译的准备率也不是很稳定，可能也会出现相差很大的语义翻译。

## 需求列表与人工智能API加值 

| 需求案例 |优先级|功能api|
|---|---|---|
|用户在不方便手记内容信息的情况下，希望快速记录准确要点|重要|百度语音识别api|
|用户希望更保险储存手写内容，在需要手动录入|次要|百度手写文字识别api|
|用户在急需文本翻译而不能快速找到相应的翻译工具|次要|百度通用翻译api、文字识别api（辅助）|

需求列表：使用人工智能的加值是否反映到需求列表（核心功能的排序上）且PRD列出明显有可行及可用的API

## 原型 
* 附件-[**产品原型**](http://kelingt.gitee.io/yang_blog)
### 原型1.交互及界面设计
#### 1. **起始页面**

![起始页面](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/启动.PNG)

#### 2. **新增内容**，点击【首页】下方圆形有“+”处，弹出选选项。选择语音时将会更据输入的语音识别之后输出文字内容，并生成新的【便签】

![新增](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/新增.PNG)

#### 3. **翻译文本**，点击【首页】下方圆形有“+”的右处图标，跳转置【翻译】页面，可直接输入文本，下方会自动输出文本，也可以点击右上角处的图标，进行文本扫描，并输出翻译内容。另外，【翻译】页面左上角，可点击选项更换翻译语言

![翻译](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/翻译.PNG)

#### 4. **手写文字转录**，点击【首页】下方圆形有“+”的左处图标，跳转至【手写转文字】页面，可直接件文本放进框中拍照识别，也可点击右上角图片输入进行相应工作

![手写](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/手写.PNG)

### 原型2.信息设计
#### 产品原型信息架构图
![信息架构图](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/信息架构图.PNG)

参考[**产品原型**](http://kelingt.gitee.io/yang_blog)

信息设计：在PRD文件中是否有说明且原型是否有做到：信息设计的某个核心信息或设计使用了人工智能的加值
### 原型3.原型文档

[**产品原型文档**](http://kelingt.gitee.io/yang_blog)

[**产品原型文档元件**](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/产品原型文档元件.rp)--下载


原型文档：多少程度上有提供MVP可交互的原型文档，供它人在Github上下载使用
### 原型4.口头操作说明
各位好，今天要介绍的是一款便捷高效的办公型人工智能产品————**智能便签**。首先进入页面，选择新建**语音输入**项，可长按输入语音，通过语音识别快速编辑文本笔记，不仅方便特殊场合的要点快速记录，同时也方便各位记录某时刻的突发奇想。另外还有一项功能，**手写文字转录**，选择这一项功能，选择拍照和图片输入，可转录大家随手在纸张上书写的文字笔记，将书写的笔记电子化，方便资料的系统化储存。最后，它还有一项**翻译**功能，选择翻译工具，输入需要翻译的文本或文件，通过机器翻译这一项人工智能，帮助大家在紧要时的外文翻译。以上便是此产品的操作简况，欢迎各位下载并使用此产品，谢谢！

口头操作说明：多少程度上在2-3分钟时间限制内，对听众留下了「的确这是个可行丶可用的人工智能加值产品」的印象
## API 产品使用关键AI或机器学习之API的输出入展示
### [API测试使用素材](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/测试材料.zip)
### API1.使用水平
1. 百度API的token的获取
```Python
#第一步先是来请求token
# access_token 的有效期为 30 天，切记需要每 30 天进行定期更换，或者每次请求都拉取新 token

# encoding:utf-8
import requests 

# client_id 为官网获取的AK=API Key， client_secret 为官网获取的SK=Secret Key
host = 'https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id=【官网获取的AK】&client_secret=【官网获取的SK】'  # Key 不要用双引号括起来只是部分参数而已
response = requests.get(host)
if response:
    print(response.json())
```
- 请求
  
  ![token请求代码图片](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/token请求.PNG)
- 返回
  ```
  {'refresh_token': '25.9df19889433fc5001cefb8446d531173.315360000.1893261598.282335-18156003', 'expires_in': 2592000, 'session_key': '9mzdDc636/G2MenMoAEPpCB2U+1QBRaRxlevU0dE5+ihGn59l1Bila0O7kHttDT961Q2Vb8SRpgZoKMHM8xoXto9Yw2DEg==', 'access_token': '24.68b90052b6cf2ba4ae6e6e141b26f43b.2592000.1580493598.282335-18156003', 'scope': 'audio_voice_assistant_get brain_enhanced_asr audio_tts_post public brain_all_scope brain_ocr_handwriting picchain_test_picchain_api_scope wise_adapt lebo_resource_base lightservice_public hetu_basic lightcms_map_poi kaidian_kaidian ApsMisTest_Test权限 vis-classify_flower lpq_开放 cop_helloScope ApsMis_fangdi_permission smartapp_snsapi_base iop_autocar oauth_tp_app smartapp_smart_game_openapi oauth_sessionkey smartapp_swanid_verify smartapp_opensource_openapi smartapp_opensource_recapi fake_face_detect_开放Scope vis-ocr_虚拟人物助理 idl-video_虚拟人物助理', 'session_secret': 'd4c94b69fc180262ffe137a01b1ec293'}
  ```
2. 语音识别api测试（核心价值）
- 代码
```Python
import requests,json,uuid,base64
token = '24.68b90052b6cf2ba4ae6e6e141b26f43b.2592000.1580493598.282335-18156003'#token请自行申请
file = open("fa.wav", "rb").read()#音频文件
url = "http://vop.baidu.com/server_api"
mac_address = uuid.UUID(int=uuid.getnode()).hex[-12:]
params = {"format": "wav",
    "lan": "zh",
    "token": token,
    "len": len(file),
    "rate": 16000,
    "speech": base64.b64encode(file).decode("utf-8"),
    "cuid": mac_address,
    "channel": 1}
headers = {"Content-Type": "application/json"}
response = requests.post(url, params=json.dumps(params), headers=headers)
if response:
    print (response.json())
```
- 返回
```
{"corpus_no":"6777113310890319637","err_msg":"success.","err_no":0,"result":["我不知道。"],"sn":"561065703321577919653"}
```
- 测试详情

|事项|错误码|报错原因|修改调整|备注|
|---|---|---|---|---|
|第一次测试|3316|使用音频为m4a格式，错误使用wav格式参数数填写方式|调整参数|-|
|第二次测试|3302|鉴权失败，请求requests_url输入错误，m4a格式音频的语音识别只有语音识别极速版可实现|修改requests_url|-|
|第三次测试（尝试多种音频格式，将m4a转mav）|3310|音频文件过大|修剪音频长度|-|

3. 手写文字识别api测试
- 代码
 ```Python
import requests,json,base64
url = "https://aip.baidubce.com/rest/2.0/ocr/v1/handwriting"
file = open("yan.png","rb").read()#图片
png = base64.b64encode(file)
params = {"image":png}
token = '24.68b90052b6cf2ba4ae6e6e141b26f43b.2592000.1580493598.282335-18156003'#token请自行申请
url = url + "?access_token=" + token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(url, data=params, headers=headers)
if response:
    print (response.json())
 ```
- 返回
```
{'log_id': 7177952755635660962, 'words_result_num': 6, 'words_result': [{'location': {'width': 368, 'top': 385, 'left': 477, 'height': 66}, 'words': '《演讲的力量》'}, {'location': {'width': 970, 'top': 452, 'left': 395, 'height': 81}, 'words': '任何一个人,只要拥有值得分享的思想,就能'}, {'location': {'width': 1019, 'top': 526, 'left': 335, 'height': 73}, 'words': '发表精彩的演讲,在公共演讲中,唯一真正重要的'}, {'location': {'width': 1025, 'top': 603, 'left': 341, 'height': 69}, 'words': '东西不是自信,不是舞台展示,也不是流利的语言'}, {'location': {'width': 434, 'top': 681, 'left': 349, 'height': 65}, 'words': '而是有价值的思想'}, {'location': {'width': 380, 'top': 740, 'left': 953, 'height': 75}, 'words': '——克里斯·安德森'}]}
```
- 测试详情

|事项|错误码|报错原因|修改调整|备注|
|--- |---|---|---|---|
|第一次测试|216101|缺少必要参数|调整参数|-|
|第二次测试（更换图片格式ipj转png）|-|-|-|无报错正常返回结果|

4. 百度通用翻译api测试
```Python
import http.client,hashlib, urllib,random,json
appid = '2020*******372015'  # 申请自己的appid
secretKey = 'MluG********KjzT'  # 申请自己的key
httpClient = None
myurl = '/api/trans/vip/translate'
fromLang = 'auto'   #填入有翻译的句子的语种，en(英),fra(法)等等
toLang = 'zh'   #译文语种，不可以填写auto
salt = random.randint(32768, 65536)# 随机数
q=open('kkk.txt').read()#输入翻译文件或梯段“q='字段'”
sign = appid + q + str(salt) + secretKey
sign = hashlib.md5(sign.encode()).hexdigest()
myurl = myurl + '?appid=' + appid + '&q=' + urllib.parse.quote(q) + '&from=' + fromLang + '&to=' + toLang + '&salt=' + str(salt) + '&sign=' + sign
try:
    httpClient = http.client.HTTPConnection('api.fanyi.baidu.com')
    httpClient.request('GET', myurl)
    response = httpClient.getresponse()
    result_all = response.read().decode("utf-8")
    result = json.loads(result_all)
    print (result)
except Exception as e:
    print (e)
finally:
    if httpClient:
        httpClient.close()
```
- 返回
```
{'from': 'en', 'to': 'zh', 'trans_result': [{'src': 'Life is full of confusing and disordering Particular time,a particular location,Do the arranged thing of ten million time in the brain,Step by step ,the life is hard to avoid delicacy and stiffness No enthusiasm forever,No unexpected happening of surprising and pleasing So,only silently ask myself in mind Next happiness,when will come?', 'dst': '生活中充满了混乱无序的特定时间、特定地点，在大脑中做着千万次的安排，一步一步，生活中难以避免的细腻和僵硬永远没有热情，所以没有意外惊喜和愉悦的发生，只有默默地问自己下一个幸福，什么时候会来？'}]}
```
- 测试详情

|事项|错误码|报错原因|修改调整|备注|
|---|---|---|---|---|
|第一次测试（字段测试‘apple’）|-|-|-|无报错正常返回结果|
|第二次测试（文件测试‘kkk.txt’）|-|-|-|无报错正常返回结果|

4. 百度文字识别api测试
- 代码
```Python
import requests,json,base64
url = "https://aip.baidubce.com/rest/2.0/ocr/v1/general_basic"
file = open("en.png","rb").read()
png = base64.b64encode(file)
params = {"image":png}#image和url各选一个
token = '24.48afc02361999d06bfdc2b067dc5a560.2592000.1580545631.282335-18160921'
url = url + "?access_token=" + token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(url, data=params, headers=headers)
if response:
    print (response.json())
```
- 返回
```
{'log_id': 8411515331957384194, 'words_result_num': 11, 'words_result': [{'words': 'ACKNOWLEDGEMENTS'}, {'words': 'We would like to thank all the designers and'}, {'words': 'contributors who have been involved in the'}, {'words': 'production of this book; their contributions'}, {'words': 'have been indispensable to its creation. We'}, {'words': 'would also like to express our gratitude to all'}, {'words': 'the producers for their invaluable opinions'}, {'words': 'and assistance throughout this project And to'}, {'words': 'the many others whose names are not credited'}, {'words': 'but have made specific input in this book, we'}, {'words': 'thank you for your continuous support'}]}
```
- 测试详情

|事项|错误码|报错原因|修改调整|备注|
|---|---|---|---|---|
|图片内文字识别（“en.png”）|-|-|-|无报错正常返回结果|

### API2.使用比较分析
#### 技术

|API|分类|比较|成熟度|准确率|使用难度|备注|
|:---:|:---|---|---|---|---|---|
|语音识别|百度|采样率固定16000,仅单声道,支持普通话/英语/少数方言/远场普通话;格式:pcm(不压缩)/wav(不压缩,pcm编码)/amr(压缩)/m4a(压缩,仅极速版)|高|中|低|[文档](https://ai.baidu.com/ai-doc/SPEECH/pk38lxi60)|
||科大讯飞|可单声&多声道;格式:wav,flac,opus,m4a,mp3;支持普通话/英语;采样率:8KHz/16KHz;精度:8bits,16bits|高|高|高|[文档](https://www.xfyun.cn/services/lfasr)|
|手写文字识别|百度|支持对图片中手写中文/数字检测识别,针对不规则的手写字体进行专项优化,识别准确率可达90%以上|高|高|低|[文档](https://ai.baidu.com/ai-doc/OCR/hk3h7y2qq)|
||科大讯飞|在识别上和百度的特性基本相同,知识百度的功能更广,可支持手画表单的识别|中|高|低|申请账户付费才可查看文档|
|机器翻译|百度|支持28种语言互译|高|高|低|[文档](http://api.fanyi.baidu.com/api/trans/product/apidoc)|
||阿里|要用于英语和法语,英语和西班牙语的互译|低|低|低|[文档](https://help.aliyun.com/document_detail/125066.html?spm=a2c4g.11186623.6.543.496121218Q2CM8)|
|文字识别|百度|可支持语种混合识别,能识别所有常用字和大部分生僻字|高|高|低|[文档](https://ai.baidu.com/ai-doc/OCR/zk3h7xz52)|
||阿里|响应快,准确率上没有百度高|中|中|低|申请账户付费才可查看文档|

#### 成本

|API|分类|比较|性价比|备注|
|:---:|:---|:---:|---|---|
|语音识别|百度|![标准版收费表](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/b_yysb.PNG)|高|[详情](https://ai.baidu.com/ai-doc/SPEECH/Jk38lxn2j)|
||科大讯飞|![收费表](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/kf_yysb.PNG)|低|[详情](https://www.xfyun.cn/services/lfasr)|
|手写文字识别|百度|![收费表](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/b_sxwzsb.PNG)|高|[详情](https://ai.baidu.com/ai-doc/OCR/Ek3h7xvq7)|
||科大讯飞|![收费表](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/kf_sxwzsb.PNG)|低|[详情](https://www.xfyun.cn/services/wordRecg)|
|机器翻译|百度|![收费表](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/b_fy.PNG)|高|在百度翻译平台申请服务才可查看收费标准|
||阿里|![收费表](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/a_fy.PNG)|中|[详情](https://help.aliyun.com/document_detail/96389.html?spm=a2c4g.11186623.6.572.4f7f4bc7SSWj3h)|
|文字识别|百度|![最普通版本收费表](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/bwzsb.PNG)|高|[详情](https://ai.baidu.com/ai-doc/OCR/9k3h7xuv6)|
||阿里|![收费表](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/img/a_wzsb.PNG)|低|[详情](https://ai.aliyun.com/ocr/general?spm=5176.12127803.1238494.6.4b756f87Ec49vL)|

#### 结论
根据各项分析，从技术综合和成本花费上，最后百度的各项api产品更适合“智能便签app”的功能开发，在最大满足技术需求的同时，保证成本保证成本的消耗不会很高。

### API3.使用后风险报告 

|API类别|市场竞争程度|输入输出限制|定价|
|:---:|:---|:---|:---|
|语音识别|科大讯飞较之百度技术承受度上高一些|百度识别的录音文件时常不超60s，小于4M，默认2-10QPS|标准版不限免费额度，极速版每个账号可免费调用5万次，极速版开通付费后为50QPS。[详细价格表](https://ai.baidu.com/ai-doc/SPEECH/Jk38lxn2j)|
|手写文字识别|相比科大讯飞百度在此技术层面上更有研究|手写文字不能过于潦草，否则将识别错误|免费额度50次/天，免费额度用尽后按照如下价格进行计费。[详细价格表单](https://ai.baidu.com/ai-doc/OCR/Ek3h7xvq7)|
|机器翻译|在市面上，百度在此方面的合作商不少，诸如一些教育类的软件如作业帮、沪江小D等，阿里的机器翻译多用于电商行业，在办公办公领域没有百度翻译的成熟|文字可直接识别翻译，图片还不能做到识别，所以需要文字识别为辅助。且不能超出可识别的语库|普通版免费额度5万次/天，超出可开通按量阶梯后付费，按次计费。[详细价格表单](https://ai.baidu.com/ai-doc/OCR/9k3h7xuv6)|



### API4.加分项 
- 语音识别api
- 手写文字识别api
- 通用翻译api
- 文本识别api
#### [代码](https://github.com/YangYuxing12345678900/API_ML_AI/blob/master/代码.md)

使用复杂度：用了2个以上机器学习与人工智能的API之输入及输出
