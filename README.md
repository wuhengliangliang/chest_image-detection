# -
详细介绍可以参考博客：https://blog.csdn.net/qq_41479464/article/details/124957629?spm=1001.2014.3001.5501

肺部图片识别使用jupyter notebook
一、整体流程
![image](https://user-images.githubusercontent.com/39480565/173019263-8fb03fe8-69e2-4787-9f56-eebccbbfcd4b.png)


![image](https://user-images.githubusercontent.com/39480565/173019404-31043d76-ada6-4a6c-a6de-8c1559dd8ae9.png)




 

案例主要流程：

第一步：加载预训练模型ResNet，该模型已在ImageNet上训练过。

第二步：冻结预训练模型中低层卷积层的参数(权重)。

第三步：用可训练参数的多层替换分类层。

第四步：在训练集上训练分类层。

第五步：微调超参数，根据需要解冻更多层。

 

ResNet 网络结构图

![image](https://user-images.githubusercontent.com/39480565/173019477-218ab1af-a19b-435d-b7af-3b7973af7e8b.png)
![image](https://user-images.githubusercontent.com/39480565/173019508-287df2c0-294a-41fb-8c69-5d9fb63e456d.png)
![image](https://user-images.githubusercontent.com/39480565/173019568-6d4940ad-b153-4237-8197-150aa69b57bd.png)


 

 
