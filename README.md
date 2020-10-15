# openCV-threshold
an easy opencv code
  
  #include <iostream>
  
  #include<opencv2/opencv.hpp>
  
  using namespace std;
  
  using namespace cv;

int main()

{
    
    VideoCapture capture(0);//从摄像头读入视频
    while(1)//循环显示每一帧
    {
        Mat frame;//Mat对象，用于存储每一帧的图像
        capture>>frame;//读取当前帧
        imshow("读取视频",frame);//显示当前帧
        waitKey(30);//延迟30ms
    }
    return 0;
}
