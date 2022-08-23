# MultiTaskLearning

1. Folder Structure :
   MTL_Models: Multi-task models. 
         |-----> DenseNet121 
         |-----> Resnet50
   STL_DepthEst: Single-task depth models.
   STL_SemanticSeg: Single-task segmentation models.
   
 2. DenseNet121 and Resnet 50 based U-Net model architecture are presented in this project.
 
 3. Resnet50 supports both with and without attention network.
 
 4. Semantic segmentaion supports both CrossEntropy based and Dice loss based losses.

 5. Four different multi-task optimisation strategies has been adapted during network training.
    1. EW - Equal weightage, L_Total = L_s* 0.5 + L_d* 0.5, W_s - segmentation weight; W_d - depth weight; L_s - Segmentation loss; L_d - Depth loss.
    2. DWA - Dynamic Weight Averaging , refer the paper, https://openaccess.thecvf.com/content_CVPR_2019/html/Liu_End-To-End_Multi-Task_Learning_With_Attention_CVPR_2019_paper.html
    3. Grad Loss - Normalized average gradient magnitude, refer the paper, https://ieeexplore.ieee.org/document/9150759
    4. Geo Loss - Geometric loss, refer the paper, refer the paper, http://openaccess.thecvf.com/content_CVPRW_2019/html/WAD/Chennupati_MultiNet_Multi-Stream_Feature_Aggregation_and_Geometric_Loss_Strategy_for_Multi-Task_CVPRW_2019_paper.html



