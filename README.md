# Tlb-yolo:Tlb yolo a rapid and efcient real time algorithm for box-type classification and barcode recognition on the moving conveying and sorting systems
Tlb yolo a rapid and efcient real time algorithm for box-type classification and barcode recognition on the moving conveying and sorting systems

⭐ This code has been completely released ⭐



# Train
1. Prepare training data
   
   1.1 Image Preprocessing： The image preprocessing process of the YOLOv8 model involves scaling the image to a specified size while preserving most of the image's features. The input image size for YOLO models is typically square, so the original image's longer side is scaled to the specified size. The shorter side is padded with pixels on both sides to make its length equal to the longer side. Due to the model's ability to adapt to images of various sizes, the padding on both sides can be reduced as long as the padded shorter side's pixel count is a multiple of the model's downsampling factor.
   ![image](https://github.com/user-attachments/assets/a57333c5-f4cd-4ef0-af3a-9bef5b1e4e3f)

    1.2 Data Augmentation: The data augmentation method used by the YOLOv8 model is the Mosaic operation. This technique randomly processes (e.g., cropping, scaling, rotating) four images and then stitches them together into a single image. Using Mosaic for data augmentation increases the diversity of the input images, effectively improving the model's generalization ability
   ![image](https://github.com/user-attachments/assets/a1029c17-7534-4887-ab24-13e7b6c8f1ad)

    1.3 The training dataset is in the trainData folder.
   
2. Begin to train multi images
   
   new fusion method MF
   
3. Begin to train RGB or IR images
4. Begin to train multi images without SR branch
5. Begin to train RGB or IR images without SR branch

 # Test
1. Pretrained Checkpoints
You can use our pretrained checkpoints for test process. Download pre-trained model and put it in here.


⭐⭐ The new weight is available at small_EDSR_MF

⭐⭐The google drive link is small_EDSR_MF

2. Begin to test

# Results
| Model                            | NoP (M) | FLOPs (G) | mAP0.5 | mAP0.95 |latency| FPS   |
|----------------------------------|:-------:|:---------:|:------:|:-------:|:----:|:-----:|
| YOLOv3-tiny                      | 8.71    | 13.0      | 42.5%  | 18.5%   | 3.2ms| 202.5 |
| YOLOv4-tiny                      | 6.11    | 17.6      | 45.3%  | 21.3%   | 3.7ms| 178.6 |
| YOLOv5n                          | 1.79    | 4.3       | 58.0%  | 35.0%   | 5.8ms| 136.8 |
| MobileNetv3-YOLOv5s              | 3.59    | 6.4       | 55.3%  | 32.6%   | 6.7ms| 121.4 |
| ShuffleNetv2-YOLOv5s             | 5.56    | 11.6      | 56.1%  | 35.4%   | 5.3ms| 151.3 |
| GhostNet-YOLOv5s                 | 3.73    | 8.2       | 63.0%  | 42.1%   | 6.0ms| 135.1 |
| YOLOv8                           | 3.8     | 6.0       | 60.2%  | 39.0%   | 6.3ms| 158.7 |
| YOLOv3-tiny slim-neck            | 5.86    | 9.6       | 56.8%  | 33.6%   | 3.0ms| 219.5 |
| YOLOv4-tiny slim-neck            | 5.66    | 16.2      | 61.3%  | 37.3%   | 3.7ms| 179.1 |
| YOLOv5n slim-neck                | 1.15    | 3.5       | 58.9%  | 37.1%   | 4.8ms| 155.4 |
| GSConv-MobileNetv3-YOLOv5s       | 9.30    | 14.1      | 61.9%  | 41.4%   | 8.3ms| 102.9 |
| GSConv-ShuffleNetv2-YOLOv5s      | 7.74    | 13.6      | 58.7%  | 37.9%   | 5.8ms| 137.1 |
| GSConv-GhostNet-YOLOv5s          | 3.73    | 8.2       | 63.6%  | 42.8%   | 6.8ms| 122.8 |
| CA-WIoU-YOLOv5s                  | 3.8     | 8.5       | 66.0%  | 42.0%   | 6.8ms| 147.1 |
| GSConv-Slimneck-CA-WIoU-YOLOv8   | 3.8     | 8.5       | 68.1%  | 44.2%   | 6.5ms| 153.8 |
| U-YOLOv8                         | 3.8     | 8.5       | 68.1%  | 44.2%   | 6.5ms| 153.8 |

 # Acknowledgements
This code is built on YOLOv8 (PyTorch). We thank the authors for sharing the codes.

 # Contact
 If you have any question, please contact me with email (shenliang@sust.edu.cn).

 
