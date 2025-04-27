# solved-disk-scheduling-algorithm
**TO GET THIS SOLUTION VISIT:** [SOLVED:Disk Scheduling Algorithm](https://www.ankitcodinghub.com/product/solveddisk-scheduling-algorithm-solution/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;3236&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SOLVED:Disk Scheduling Algorithm&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Aim

The main aim of this program is to become more familiar with hard disk file system scheduling concepts. We will do this by writing a program to simulate head movement with FCFS (First Come First Served), SSTF (Shortest Seek Time First), SCAN, CSCAN (Circular SCAN), LOOK and CLOOK (Circular LOOK) Scheduling algorithms.

In class we examined various disk scheduling algorithms all of which have various advantages and disadvantages depending on load and conditions. For this assignment you are to write a program that simulates the head movement of the hard disk with different disk scheduling algorithms, namely: FCFS, SSTF, SCAN, CSCAN, LOOK and CLOOK.

Your program should prompt for the starting cylinder, the current head direction (i.e. ‘L’ or ‘l’ if the direction is toward cylinders less than the starting position and ‘G’ or ‘g’ if the direction is toward cylinders greater than the starting cylinder), and the cylinder request queue (i.e. all the cylinders to be read in the order requested).

For each algorithm your program should compute and display the head movement (i.e. the order in which the cylinders are visited based on the current algorithm), the total head movement (in cylinders) based on the current algorithm and the max and min waiting time for the disk requests.

You can assume: The disk has 200 cylinders commencing from 0 to 199. All disk requests are queued and waiting for the disk scheduler. The disk’s seek time is 0.8ms per cylinder and the rotational latency is 3ms average. With CSCAN and CLOOK the ‘L’ direction causes flyback from cylinder 0 (or min request) to 199 (or max request) and visa versa the ‘G’ direction. For FCFS and SSTF the head direction is ignored.

An example interaction is shown below. (Note: bold text indicates user input. The output shown is for format purposes only. i.e. it is not correct.)

Cylinder Start: **53**

Head Direction: **g**

Cylinder Queue: **98 183 37 122 14 124 65 67**

“`cpp

FCFS Head Movement: 53=98=183=37=122=14=124=65=67

FCFS Total Movement: 640 cylinders

FCFS Min Waiting Time: 55ms

FCFS Max Waiting Time: 220ms

FCFS Ave Waiting Time: 110ms

SSTF Head Movement: 53=65=67=37=14=98=122=124=183

SSTF Total Movement: 640 cylinders

SSTF Min Waiting Time: 35ms

SSTF Max Waiting Time: 260ms

SSTF Ave Waiting Time: 120ms

…..

…..

BEST TO WORST ALGORITHMS (min to max)

Total Cylinders: SSTF LOOK CLOOK SCAN CSCAN FCFS

Max Waiting Time: LOOK CLOOK SSTF CSCAN SCAN FCFS

Ave Waiting Time: SSTF LOOK CLOOK SCAN CSCAN FCFS

“`

You can assume all input (except head direction) are integers. When invalid input is detected the whole line of input should be requested again. (One suggestion is to read the whole line with getline() and extract the integers with sscanf() or a stringstream).
