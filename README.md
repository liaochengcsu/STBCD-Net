# STBCD-Net
Building change detection based on single-temporal high-resolution remote sensing imagery (HRSI)

## Abstract

Buildings are fundamental structures closely intertwined with human activity. Detecting changes in buildings is of significant importance for land cover investigation, dynamic urban expansion, illegal building monitoring, etc. Current approaches primarily concentrate on analyzing differences in bi-temporal remotely sensed imagery. However, pseudo-changes, such as variations in non-building elements due to different illumination and seasons, along with offsets in corresponding buildings caused by diverse sensor attitudes, present considerable challenges for reliable building change identification. To address these issues, we propose a novel learning-based multi-head building change detection network (ST-BCD) that leverages historical building polygons and single-temporal imagery. Firstly, we design a multi-head decoder to disentangle fused multi-scale features extracted from a pre-trained encoder, enabling separate extraction of newly added and removed buildings. Subsequently, we introduce an instance-level contrastive loss to enhance the global distinctiveness between building and non-building features. Additionally, we present a random label generation strategy to mitigate the issue of unbalanced change labels. Overall, we transform change detection based on discriminative features of bi-temporal imagery into a multi-task building segmentation approach using single-temporal imagery. We evaluate the effectiveness of our proposed method on the WHU-CD and private building change detection datasets. The experimental results demonstrate the superiority of our approach, achieving F1-scores of 93.81% and 68.36% on the above datasets, respectively. 
<div align=center><img width="500" height="550" src="https://github.com/liaochengcsu/pics/figure1.png"></div>


## DataSets

<div align=center><img width="600" height="400" src="https://github.com/liaochengcsu/BCE-Net/blob/main/pics/figure10.png"/></div>

+ The modified WHU-CD Dataset: Download at [WHU-CD-Baiduyun](https://pan.baidu.com/s/1lceyKsCTcqw2Neq1FUzh9w) with extract code: c9a4. It contains 1260 and 690 sliced tiles same as the [Offcial Webset](http://gpcv.whu.edu.cn/data/building_dataset.html)   
<div align=center><img width="600" height="350" src="https://github.com/liaochengcsu/BCE-Net/blob/main/pics/figure9.png"/></div>

+ The ST-BCD Dataset: Download at [ST-BCD-Baiduyun](https://pan.baidu.com/s/1Um2nnbCXDtQXMhiWJR1d3A) with extract code: 5gyh.  It contains 3604 and 1328 sliced tiles for training and test dataset.
