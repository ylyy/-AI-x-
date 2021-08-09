比赛背景

第三届中国AI+创新创业大赛由中国人工智能学会主办，半监督学习目标定位竞赛分赛道要求选手基于少量有标注数据训练模型，使分类网络具有目标定位能力，实现半监督目标定位任务。

中国人工智能学会（Chinese Association for Artificial Intelligence，CAAI）成立于1981年，是经国家民政部正式注册的我国智能科学技术领域唯一的国家级学会，是全国性4A级社会组织，挂靠单位为北京邮电大学；是中国科学技术协会的正式团体会员，具有推荐“两院院士”的资格。

中国人工智能学会目前拥有51个分支机构，包括43个专业委员会和8个工作委员会，覆盖了智能科学与技术领域。学会活动的学术领域是智能科学技术，活动地域是中华人民共和国全境，基本任务是团结全国智能科学技术工作者和积极分子通过学术研究、国内外学术交流、科学普及、学术教育、科技会展、学术出版、人才推荐、学术评价、学术咨询、技术评审与奖励等活动促进我国智能科学技术的发展，为国家的经济发展、社会进步、文明提升、安全保障提供智能化的科学技术服务。

中国“AI+”创新创业大赛由中国人工智能学会发起主办，是为了配合实施创新驱动助力工程，深入开展服务企业技术创新活动，进一步提高我国文化建设和实践创新能力，展示智能科学与技术等相关学科建设的新经验、新成果，促进专业内涵的建设而发起的综合性大赛平台。

飞桨PaddlePaddle作为中国首个自主研发、功能完备、开源开放的产业级深度学习平台，为本次比赛的参赛选手提供了集深度学习核心训练和推理框架、基础模型库、端到端开发套件和丰富的工具组件于一体的一站式服务。百度大脑AI Studio作为官方指定且唯一的竞赛日常训练平台，为参赛选手提供高效的学习和开发环境，更有亿元Tesla V100算力免费赠送，助力选手取得优异成绩。

比赛链接
https://aistudio.baidu.com/aistudio/competition/detail/78

简要介绍

赛题背景

半监督学习(Semi-Supervised Learning)是指通过大量无标记数据和少量有标记数据完成模型训练，解决具有挑战性的模式识别任务。近几年，随着计算硬件性能的提升和大量大规模标注数据集的开源，基于深度卷积神经网络(Deep Convolutional Neural Networks, DCNNs)的监督学习研究取得了革命性进步。然而，监督学习模型的优异性能要以大量标注数据作为支撑，可现实中获得数量可观的标注数据十分耗费人力物力(例如，获取像素级标注数据)。于是， 半监督学习逐渐成为深度学习领域的热门研究方向，只需要少量标记数据就可以完成模型训练过程，更适用于现实场景中的各种任务。

比赛任务
本次比赛要求选手基于少量有标签的数据训练模型，使分类网络具有目标定位能力，实现半监督目标定位任务。每- -位参赛选手仅可以使用ImageNet大型视觉识别竞赛(LSVRC)的训练集图像作为训练数据，其中有标签的训练数据仅可以使用大赛组委会提供的像素级标注。
本次比赛项目的目录结构如下

main.ipnb:运行主代码的notebook文件

data:比赛数据集
    -dataxxxxx:
          -dataset.zip #这个是压缩包的训练集
         -B榜测试数据集.zip

    -image #dataset.zip 解压后产生
    -mask #dataset.zip 解压后产生
    -test_image #dataset.zip 解压后产生

运行完程序后会出现新的文件夹

paddleseg：从paddle下载的图像分割套件

ocrnet.yml:训练参数的配置文件

output:最终提交的的预测图

本项目最终B榜成绩0.764
