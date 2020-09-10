# Dilated Evolving Attentive Spatial-Frequency Network
    Seeing the Unseen: 
    Wifi-based 2D Human Pose Estimation via Dilated Evolving Attentive Spatial-Frequency Network


* [Architecture](#architecture)

* [Dataset](#dataset)

* [Visulization](#visulization)

* [Result](#result)

## Architecture
![image](https://github.com/DEASFN/DEASFN/blob/master/pic/architecture.png)

## Dataset
Place | Type | Url | Place | Type | Url
:---:| :---: | :---: | :---:| :---: | :---:
P1 | single-person 01 | https://reurl.cc/oLE0bV | P1 | single-person 02 | https://reurl.cc/E75GNa
P1 | single-person 03 | https://reurl.cc/MvKRmm | P1 | single-person 04 | https://reurl.cc/ZOLWjM
P1 | single-person 05 | https://reurl.cc/z8nYW6  | P1 | single-person 06 | https://reurl.cc/1xN1oV
P1 | multi-people | https://reurl.cc/9EmVA8 | P1 | wall | https://reurl.cc/WdKDY5
P2 | single-person 01 | https://reurl.cc/5l9MyR | P2 | single-person 02 | https://reurl.cc/62nN3k
P2 | single-person 03 | https://reurl.cc/j7Klj2 | P2 | single-person 04 | https://reurl.cc/b5K9V6
P2 | single-person 05 | https://reurl.cc/3DqxXL | P2 | single-person 06 | https://reurl.cc/exKDzm
P2 | multi-people | https://reurl.cc/4RVQ7V 


## Visulization
### Comparative  visualization  of  DEASFN  and  two models (PIW[2] and WiSPPN[1])
![image](https://github.com/DEASFN/DEASFN/blob/master/pic/comparison.png)

### Some positive cases of DEASFN on our two benchmarks
![image](https://github.com/DEASFN/DEASFN/blob/master/pic/demo.png)


## Result
The PCK@20(Percentage of Correct Keypoint)of provided models are shown here:
|Method|single-person|multi-people|                       
| :------| :------: | :------: |
|WiSPPN[1]|  69.82%    | X   |
|Person-in-WiFi[2] | 77.06% | 61.58%|
|**MDT-GCN(ours)**|**82.26%**|**71.58%**|

|Method|through-wall|
| :------| :------: |
|WiSPPN[1]|  58.86%    |
|Person-in-WiFi[2] | 73.67%|
|**MDT-GCN(ours)**|**80.72**%|


[1] Fei Wang, Stanislav Panev, Ziyi Dai, Jinsong Han, and Dong Huang. 2019. Canwifi estimate person pose?arXiv preprint arXiv:1904.00277(2019).

[2] Fei Wang, Sanping Zhou, Stanislav Panev, Jinsong Han, and Dong Huang. 2019.Person-in-WiFi: Fine-grained person perception using WiFi. InProceedings of theIEEE International Conference on Computer Vision. 5452–5461.
