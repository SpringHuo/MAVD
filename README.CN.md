## <center>MAVD: The First Open Large-Scale Mandarin Audio-Visual Dataset with Depth Information</center>
### 简介
为了解决中文普通话领域内开源数据集数量少、数据质量较差的问题，我们团队制作了本数据集MAVD。MAVD是一个多模态数据集，包含文本、音频、视频等模态，特别地是，MAVD使用了微软最新的深度相机Azure Kinect，同步采集了相应的深度图像，以期探究深度图像在多模态任务中的帮助。

MAVD中包含了64位说话人阅读的12484条数据，总时长约为24小时。其中说话人包括35位男性以及29位女性说话人，平均年龄为23岁。阅读材料为我们精心挑选的文本语句，采集自在中文使用场景下的众多开源媒体（微博、豆瓣、人民日报等）。涵盖了日常生活类、新闻类、小说类以及古诗词四个不同主题。在采集所有的生语料之后，我们进行了文本的清洗以及筛选，并在最后经过了人工审查。各个主题占比粗略为10:5:4:1。

<p align="center" width="100%">
    <img width="40%" src="image/speakers.png"> 
</p>

MAVD采集自可以隔绝外部噪声并且吸收回音的静音室中，具体的场景设置如下图所示。所有采集人员使用我们所开发的多模态数据采集系统进行数据录制，每位说话人阅读约200句语句。最后，在录制结束后，我们对所有数据进行了检查以及挑选，并且通过MFA对语音进行了音素级的标注。更加详细的介绍可以关注我们在InterSpeech2023中所介绍的论文。

<p align="center" width="100%">
    <img width="40%" src="image/setting.jpg"> 
</p>

<p align="center" width="100%">
    <img width="33%" src="image/setting2.jpeg"> 
</p>

### 数据集结构
在本项目中，上传了单条语句示例，MAVD具体的数据结构如下图所示。数据集中说话人编号为 F/M+XX 的方式来区分性别以及具体序号。每个说话人对应4个文件夹，其中“AUDIO”中保存为说话人阅读语句相应的音频文件，格式为“xxx.wav”，采样率为16kHZ；“COLOR\_IMAGE”中保存每条语句的RGB图像序列，图像格式为“xxx\_xxxxxxxxx\_color.jpg”，其中前3位为图像序号，后9位为图像时间戳，分辨率为1920 x 1080，30fps；“DEPTH\_IMAGE” 与RGB图像保存格式类似，深度图像分辨率为 640 x 576；“TEXT”中保存该句文本、拼音以及语音标注文件。

<p align="center" width="100%">
    <img width="33%" src="image/tree.png"> 
</p>

### 目前情况以及获取方式
MAVD数据集已完成清洗和整理，目前开发下载，如您有获取数据集的需要，请联系天津大学毕老师（邮箱：***\*bkb@tju.edu.cn\****）进行数据集获取。注意，请先下载并填写相关申请表。

#### 联系方式：bkb@tju.edu.cn、avrillliu@hkust-gz.edu.cn、yuchenhuo@tju.edu.cn
