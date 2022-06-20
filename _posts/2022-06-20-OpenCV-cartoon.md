---
layout: single
title: "opencv chapther04"
---
# openCV에서 비디오 캡쳐 resize 하는 방법
```
import cv2

def print_howto():
    print("""
        Change color space of the input video stream using keyboard controls. 
        The control keys are: 
            1. Grayscale    - press 'g'
            2. YUV          - press 'y'
            3. HSV          - press 'h'
            4. RGB          - press 'r'
    """)


if __name__=='__main__':
    print_howto()
    cap = cv2.VideoCapture(0)

    if not cap.isOpened():
        raise IOError("Cannot open webcam")
    cur_mode = None
arr = []
while True:
    ret, frame = cap.read()
    frame = cv2.resize(frame, None, fx=0.5, fy=0.5, interpolation=cv2.INTER_AREA)
    c = cv2.waitKey(1)

    if c == 27:
        break
    if c != -1 and c != 255 and c != cur_mode:
        cur_mode = c

    if cur_mode == ord('g'):
        cv2.putText(frame, 'Grayscale', (50, 50), cv2.FONT_HERSHEY_DUPLEX, 1, (255, 255, 255))
        arr = 'g'
        output = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

    elif cur_mode == ord('y'):
        cv2.putText(frame, 'YUV', (50, 50), cv2.FONT_HERSHEY_DUPLEX, 1, (255, 255, 255))
        arr = 'y'
        output = cv2.cvtColor(frame, cv2.COLOR_BGR2YUV)

    elif cur_mode == ord('h'):
        cv2.putText(frame, 'HSV', (50, 50), cv2.FONT_HERSHEY_DUPLEX, 1, (255, 255, 255))
        arr = 'h'
        output = cv2.cvtColor(frame, cv2.COLOR_BGR2HSV)

    elif cur_mode == ord('r'):
        cv2.putText(frame, 'RGB', (50, 50), cv2.FONT_HERSHEY_DUPLEX, 1, (255, 255, 255))
        arr = 'r'
        output = frame
    else:
        cv2.putText(frame, 'Wrongg input', (50, 50), cv2.FONT_HERSHEY_DUPLEX, 1, (255, 255, 255))
        if arr == 'g' :
            output = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
        elif arr == 'y' :
            output = cv2.cvtColor(frame, cv2.COLOR_BGR2YUV)
        elif arr == 'h' :
            output = cv2.cvtColor(frame, cv2.COLOR_BGR2HSV)
        elif arr == 'r' :
            output == frame
        else :
            output = frame

    cv2.imshow('Webcam', output)


cap.release()
cv2.destroyAllWindows()
```
