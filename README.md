# YoloV5_PCB
This reposi tries to make a SIMPLE YoLoV5 which is used to detect the issue that appear on PCB surface.
1) The original source: https://github.com/MBDNotes/YOLOv5_PCB_Defects_Detection/tree/main
2) The github which is used to tran xml->txt: https://github.com/isabek/XmlToTxt
3) Dataset used: https://www.kaggle.com/datasets/akhatova/pcb-defects
## First: Prepare Data
### Use the XmlToText
- Copy all name of classes into classes.txt : 
missing_hole
mouse_bite
open_circuit
short
spur
spurious_copper
- Run: !python xmltotxt.py -c classes.txt -xml xml -out out
(Note: os.chdir right directory before running)
### Train
