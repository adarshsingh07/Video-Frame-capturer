# Video-Frame-capturer
Uses python language to capture from an Video. 
 #python code for playing a video using open cv
import numpy as np
import cv2

cap=cv2.VideoCapture('Sample_Video1.mp4')

while(True):
    ret, frame=cap.read()
    cv2.imshow('output',frame)
    
    if(cv2.waitKey(1) & 0xFF == ord('q')):
        break
cap.release()
cv2.destroyAllWindows
