import cv2
cap=cv2.VideoCapture(0)
cap.set(1,640)
cap.set(4,400)

while True:
    success, img= cap.read()
    cv2.imshow("Webcam",img)
    if cv2.waitKey(1) & 0xFF == ord("w"):
        break
