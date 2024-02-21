# Some useful stuff for Human Fall Detection

Из того, что удалось накопать за неделю, приличным показались следующие варианты подходов и датасетов.

### Four main approaches:

| Type         | What's Used                                 | Link                                                       | Additional Notes                                                       |
| ------------ | ------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------------------- |
| LSTM-based   | openpifpaf -> LSTM                          | https://github.com/taufeeque9/HumanFallDetection           | code for a paper; multi-person, multi-camera, ligthweight (relatively) |
| YOLO-based   | AlphaPose -> ST-GCN -> oneclass tiny YOLO | https://github.com/GajuuzZ/Human-Falling-Detect-Tracks     | weights not accessible                                                 |
| ImProc-based | openCV Haar Cascades                        | https://github.com/EikeSan/video-fall-detection            | super lightweight and super easy                                       |
| YOLO-based   | YOLOv7-POSE                                 | https://github.com/Y-B-Class-Projects/Human-Fall-Detection | heavyweight, but very nice results                                     |

some notes:

- LSTM got dependency issues. don't install reqs right away, install python 3.8, openpifpaf 0.12.14 and torchvision 0.13.0



### Datasets:

| Name               | Link                                                             | Additional Notes                                                                             |
| ------------------ | ---------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| UP Fall Detection  | https://sites.google.com/up.edu.mx/har-up                        | preprocessing: colab.research.google.com/drive/1PbzVZnwBzFK_CcMf5G3dFrjwKZgfK3Vy?usp=sharing |
| Le2i dataset       | https://universe.roboflow.com/new-workspace-qfcus/le2i/dataset/2 | many classes, 4 locations                                                                    |
| Repo with datasets | https://github.com/YifeiYang210/Fall_Detection_dataset           | some datasets are unavailable                                                                |
