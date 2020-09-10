# Dilated Evolving Attentive Spatial-Frequency Network
    Seeing the Unseen: 
    Wifi-based 2D Human Pose Estimation via Dilated Evolving Attentive Spatial-Frequency Network


* [Architecture](#architecture)

* [Dataset](#dataset)

* [Visulization](#visulization)

* [Result](#result)

* [Reference](#reference)


## Architecture
![image](https://github.com/DEASFN/DEASFN/blob/master/pic/architecture.png)

## Dataset

<table>
    <tr>
        <td colspan="2" align="center">GPE</td> 
        <td colspan="2" align="center">SPE</td> 
   </tr>
    <tr>
        <td align="center"># Person</td>
        <td align="center">Number</td>
        <td align="center">Action</td>
        <td align="center">Number</td>
    </tr>
    <tr>
        <td align="center">1</td>
        <td align="center">12,884</td>
        <td align="center">Walk</td>
        <td align="center">78,852</td>
    </tr>
    <tr>
        <td align="center">2</td>
        <td align="center">18,879</td>
        <td align="center">Wave</td>
        <td align="center">77,431</td>
    </tr>
    <tr>
        <td align="center">3</td>
        <td align="center">27,694</td>
        <td align="center">Jump</td>
        <td align="center">40,670</td>
    </tr>
    <tr>
        <td align="center">>=4</td>
        <td align="center">28,178</td>
        <td align="center">Run</td>
        <td align="center">41,238</td>
    </tr>
    <tr>
        <td align="center"><b>Total</b></td>
        <td align="center"><b>87,635</b></td>
        <td align="center"><b>Total</b></td>
        <td align="center"><b>238,191</b></td>
    </tr>
    
</table>

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
#### Comparative visualization of DEASFN and two models (PIW[2] and WiSPPN[1])
![image](https://github.com/DEASFN/DEASFN/blob/master/pic/comparison.png)

#### Some positive cases of DEASFN on our two benchmarks
![image](https://github.com/DEASFN/DEASFN/blob/master/pic/demo.png)


## Result
* The PCK@20(Percentage of Correct Keypoint)of provided models are shown here:

<table>
    <tr>
        <td align="center">Metric</td> 
        <td align="center">Benchmark</td> 
        <td align="center">WiSPPN[1]</td> 
        <td align="center">PIW[2]</td> 
        <td align="center"><b>DEASFN</b></td> 
   </tr>
    <tr>
        <td align="center" rowspan='2'>MPJPE</td>
        <td align="center">SPE</td>
        <td align="center">44.16</td>
        <td align="center">78.88</td>
        <td align="center"><b>37.34</b></td>
    </tr>
    <tr>
        <td align="center">GPE</td>
        <td align="center">X</td>
        <td align="center">119.60</td>
        <td align="center"><b>44.14</b></td>
    </tr>
    <tr>
        <td align="center" rowspan='2'>PCK@20</td>
        <td align="center">SPE</td>
        <td align="center">21.86%</td>
        <td align="center">32.96%</td>
        <td align="center"><b>50.05%</b></td>
    </tr>
    <tr>
        <td align="center">GPE</td>
        <td align="center">X</td>
        <td align="center">27.64%</td>
        <td align="center"><b>43.98%</b></td>
    </tr>
</table>

* The PCK@20(Percentage of Correct Keypoint)of provided models are shown here:

|Action|WiSPPN|PIW|**DEASFN**|                       
| :------| :------: | :------: | :------: |
|Walk|23.58%|39.87%|**61.14%**|
|Wave|25.92%|33.06%|**45.81%**|
|Jump|22.12%|37.91%|**58.11%**|
|Run|15.82%|20.99%|**35.15%**|



## Reference
* [1] Fei Wang, Stanislav Panev, Ziyi Dai, Jinsong Han, and Dong Huang. 2019. Can wifi estimate person pose?arXiv preprint arXiv:1904.00277(2019).
* [2] Fei Wang, Sanping Zhou, Stanislav Panev, Jinsong Han, and Dong Huang. 2019.Person-in-WiFi: Fine-grained person perception using WiFi. InProceedings of theIEEE International Conference on Computer Vision. 5452–5461.
