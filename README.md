# Crashlytics
## Crashlytics in Firebase  
--- 
* Crashlytics: Crash 내용 확인, 내부를 확인해도 Memory
  * ![image](https://user-images.githubusercontent.com/43035817/125762517-b05392a4-73b8-4a0a-905a-361620fcbbd4.png)
  * log1
![image](https://user-images.githubusercontent.com/43035817/125762599-8e1a2936-4f2e-49b2-8922-364d6a936b7d.png)
  * log2
![image](https://user-images.githubusercontent.com/43035817/125764653-f9f0ea6f-3c20-499f-9a9b-0a56c64bc554.png)

* download dSYM file > upload to firebase
![image](https://user-images.githubusercontent.com/43035817/125764327-18167c43-55bf-479f-9370-776f4b5ca542.png)

## Instrument
--- 
* analyze allocation graph: Memory leak이 존재하는 곳이 많으며, allocation이 솟아오르는 부분이 존재
  * ![image](https://user-images.githubusercontent.com/43035817/125764745-aefbbed4-bcb0-466a-bfa8-839ad956415e.png)

* analyze call tree: 위에서 Memory leak포인트가 있었고 Call tree 확인 결과, 다양한 곳에서 crash 발생하여 memory leak으로 인한 crash발생으로 파악
  * ![image](https://user-images.githubusercontent.com/43035817/125764424-39937484-388f-486d-943f-b403e6d054bb.png)

  * ![image](https://user-images.githubusercontent.com/43035817/125764833-b764d603-2b36-475a-8ad6-5075b3568984.png)
