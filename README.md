# 项目名称：智能毕业纪念APP    
  
### 加值宣言       
运用高德地图API，地标定位，百度人工智能API :  语音识别，人脸识别，打造一个不一样的毕业纪念册。 
产品用户群体：大学刚毕业的学生   
用户需求：在毕业季能够记录、分享当下。    
公司资源。   
市场很大，公司资源小，怎么缩小，优先级是什么。    

### 核心价值    
产品具体是为大学毕业生记录当下，留下纪念，，增加毕业趣味性，减少伤感。    
    
### 核心价值与用户痛点       
社交 分享 纪念    
传统的毕业纪念册没有新意。   

### 人工智能概率性与用户痛点   
百度语音识别：
采用领先国际的流式端到端语音语言一体化建模方法，融合百度自然语言处理技术，近场中文普通话识别准确率达98%。   

 
### 需求列表与人工智能API加值     
  
实现：   
①     
需求：社交 分享 纪念   
场景：可上传照片，在校园内任一位置打卡留念。用户可以在校园地图上查看自己或者他人的照片，也可选择是否公开自己的照片。   
②   
需求：社交、分享、记录   
场景：可分享邀请链接，邀请老师和亲朋好友留言，毕业纪念APP可将留言转换为文字和语音。   
③   
需求：划分区域   
场景：可以查看同专业同班毕业集体照，单击人物头像可显示姓名和联系方式。非同专业班级不可。   

如何实现：   
①   
使用高德地图api（地标定位），输入图片，在校园地图上输出图片   
②   
使用语音识别API，输入语音，输出文字+语音   
③   
使用人脸识别，输入图片，输出文字信息    


### 原型     
原型制作规划 测试    
### API 产品使用关键AI或机器学习之API的输出入展示    
[百度AI语音识别]([https://ai.baidu.com/tech/speech](https://ai.baidu.com/tech/speech)
)：   

输入：   
```
from aip import AipSpeech

""" 你的 APPID AK SK """
APP_ID = '18090119'
API_KEY = 'YtE6uqVodwVwr9zCW0sPjqrH'
SECRET_KEY = 'RGzlYQaeApOcXKmyjRfeKLEV02lKDlvn'

client = AipSpeech(APP_ID, API_KEY, SECRET_KEY)

# 读取文件
def get_file_content(filePath):
    with open(filePath, 'rb') as fp:
        return fp.read()

# 识别本地文件
client.asr(get_file_content('16k.pcm'), 'pcm', 16000, {
    'dev_pid': 1536,
})
```
输出：
```
{'corpus_no': '6773611276171315400',
 'err_msg': 'success.',
 'err_no': 0,
 'result': ['北京科技馆'],
 'sn': '726787071901577104272'}
```
讯飞AI语音听写：   
![讯飞语音听写](https://upload-images.jianshu.io/upload_images/11043770-9581753eb4f7bbe0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)   <br><br>

### 涉及API的价值主张    
高德地图API，地标定位   
百度API :   
语音识别   
人脸识别   
