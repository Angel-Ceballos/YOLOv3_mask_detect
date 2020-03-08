# YOLOv3-face-mask-detection
Face mask detection using YOLOv3 on Google colab

#### Photo
![image](https://github.com/VictorLin000/YOLOv3_mask_detect/blob/master/Mask/demo/predictions.jpg)

#### Video
![image](https://github.com/VictorLin000/YOLOv3_mask_detect/blob/master/Mask/demo/predictions3.gif)

### Usage
#### train
    ./darknet detector train "/content/darknet/Mask/obj.data" "/content/darknet/Mask/yolov3_mask.cfg" "/content/darknet/weights/darknet53.conv.74" -dont_show
#### detect photo
    ./darknet detect Mask/yolov3_mask.cfg weights/yolov3_mask_last.weights Mask/Mask_121.jpg
#### detect video
    ./darknet detector demo /content/darknet/Mask/obj.data Mask/yolov3_mask.cfg /content/darknet/weights/yolov3_mask_last.weights -dont_show /content/darknet/Mask/Mask_test_v_3.mp4 -i 0 -out_filename predictions.avi
    
### Reference
* https://pjreddie.com/darknet/yolo/
* https://chtseng.wordpress.com/2018/09/01/%E5%BB%BA%E7%AB%8B%E8%87%AA%E5%B7%B1%E7%9A%84yolo%E8%BE%A8%E8%AD%98%E6%A8%A1%E5%9E%8B-%E4%BB%A5%E6%9F%91%E6%A9%98%E8%BE%A8%E8%AD%98%E7%82%BA%E4%BE%8B/
* http://blog.ibanyez.info/download/B20190410T000000072.png
* https://colab.research.google.com/drive/1lTGZsfMaGUpBG4inDIQwIJVW476ibXk_#scrollTo=v3nkYzWwMuBk
* https://colab.research.google.com/drive/1EA0x98UdBqCzbW25aPUkxZkZPMRJHlsz#scrollTo=8T8AKZiy1zep&forceEdit=true&sandboxMode=true
* https://medium.com/@artinte7/real-time-object-detection-using-yolo-upon-google-colab-in-5-minutes-fd65a4903df5
