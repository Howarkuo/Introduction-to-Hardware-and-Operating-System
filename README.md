# Introduction to Hardware and Operating System
[Visit MY Hackmd.io](https://hackmd.io/@Zg_bDsGbQhaDrJGN2Sgm4Q/r1dF4YHLZe)
## 0. System Specifications (HP EliteBook 840 G6)

### Dashboard Overview
* **Storage:** 257 GB of 477 GB used
* **Graphics:** Intel(R) UHD Graphics 620
* **Memory Speed:** 2400 MT/s
* **Processor Base/Boost:** 1.60GHz / 1.90 GHz

### Device Specifications
* **Device name:** DESKTOP-OC302KO
* **Processor:** Intel(R) Core(TM) i5-8365U CPU @ 1.60GHz (1.90 GHz)
* **Installed RAM:** 16.0 GB (15.8 GB usable)
* **Device ID:** 61CA66C7-7266-4609-9063-B0EBA71949D4
* **Product ID:** 00330-52232-98653-AAOEM
* **System type:** 64-bit operating system, x64-based processor
* **Pen and touch:** No pen or touch input is available for this display


### Evaluating Computer System
Laptop Comparison: Portable, Versatile, and High-Performance Models

| Model | Use Case | Processor | RAM | Storage | Display |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **ThinkPad X13 Gen 6** | Portable Professional | Intel (Integrated Arc Graphics) | 16 GB LPDDR5x | 256 GB SSD (PCIe Gen4) | 13.3" WUXGA (1920 x 1200) IPS |
| **Dell Vostro 14 / Latitude 5440** | Balanced Professional | Not Specified | 16 GB DDR5 | 512 GB SSD | 14" FHD+ (1920 x 1200) |
| **ThinkBook 14 Gen 7** | Versatile Workhorse | AMD Ryzen™ 5 7000/8000 | 16 GB DDR5 | 512 GB SSD | 14" WUXGA Anti-glare |
| **Dell Inspiron 16** | Large-Screen Value | Intel® Core™ i5-1335U | 16 GB LPDDR5x | 512 GB SSD | 16" 16:10 Aspect Ratio |
| **ThinkPad T14s Gen 6** | Performance Powerhouse | Intel® Core™ Ultra 7 (S2) | 32 GB LPDDR5x | 1 TB SSD (PCIe Gen4) | 14" 2.8K OLED / Low Power IPS |
| **Dell Precision 7780** | Desktop Replacement | Intel® Core™ i7-13850HX | 32 GB (Up to 128 GB) | 1 TB PCIe Gen4 SSD | 17.3" FHD or 4K |

## 1. Computer Fundamentals
### Notation System
####  Notation system - decimal**
use the base of 10, a decimal marker to note fraction, display minus sign to left of negative number 
####  Notation system - binary
use 0,1 off and on state, in bits (single digit) and bytes (8 digit and no spaces e.g: 010101)
#### Convert decimal to binary
Divide the number and the quotient by 2: 
e.g: 25 /2 =12..1, 12/2 = 6..0 , 6/2 = 3..0, 3/2=1..1,1/2=0..1 
25 -> 11001
#### Convert binary to decial / Doubling method
010010 
start with eh leftmost binary number 
multiply the resulting number by 2
add the number to its right
repeat the process for each binary digit, going from left to right

(0 x 2) + 0 = 0
(0 x 2) + 1 = 1
(1 x 2) + 0 = 2
(2 x 2) + 0 = 4
(4 x 2) + 1 = 9
(9 x 2) + 0 = 18

### Operating system
1955 - 1965: IBM 704 / Embedded operating system / Real-time operating system
1965 - 1980: Network operating system , UNIX-symmetric multiprocessing, 
1980 - now: Multitasking os : Linux(RedHat) ,Windows(DiskOperating System -DOS),  macOS, Chrome OS / Mobile operating system :Android, iOS, ChromeOS, Windows 

### Linux and Distribution
**
- Foundation/ Engine Blueprint talks to the hardware : Linux
- Corporate Skyscrapers: Commercial giants
    - RHEL (Red Hat Enterprise Linux): The high-security bank vault. It’s expensive and requires a subscription, but it’s incredibly stable.
    - AlmaLinux: A "copy" of the bank vault. It uses the exact same blueprints as RHEL but is free. It’s perfect for companies that want RHEL’s stability without the high rent.
    - SUSE: The German-engineered factory. Extremely precise and popular in European industrial sectors.
- The Popular Neighborhoods (Debian, Ubuntu, Linux Mint)
    - Debian: The Stone Foundation. It is one of the oldest and most stable neighborhoods. It doesn't change often, but it almost never breaks.

    - Ubuntu: The Busy Metro Area. Built on Debian's foundation, it’s the most popular neighborhood for Data Scientists. It’s modern, has great public services (software support), and is easy to move into.

    - Linux Mint: The Comfy Suburban Home. It’s built on Ubuntu but feels more familiar to people moving from "Windows City." It’s polished and comes with everything already set up.
#### The Specialized Workshops, DIY Garage and the Tiny Home. (Arch ARM, Alpine)

Arch Linux ARM: This is a Box of Parts. You have to build the house yourself, brick by brick. The "ARM" part means it’s specifically designed for small, efficient engines (like the chips in a Raspberry Pi or the M4 Mac).

Alpine Linux: The Ultra-Minimalist Pod. It is tiny, stripped of all luxuries, and designed only for one thing: getting a specific job done as fast as possible (usually inside "containers" or virtual boxes).

#### 5. The Interior Design (GNOME)
 GNU Network Object Model Environment, Interior Design style (Desktop Environment). It’s how the buttons, windows, and menus look. GNOME is like a modern art gallery: very clean, minimalist, and uses "Workspaces" instead of a traditional Start menu.

#### 6. Specialized Purposes: 
Install on a USB disk: Tails OS (The Burner Pop-Up Tent)
isolated app and task into virtual machine: Qubes OS (The Maximum-Security Quarantine Lab)

### Linux and Architecture
#### 1. Unix: The Ancient Royal Blueprint
The Metaphor: The Original Forbidden City.
Back in the 1970s, Unix was the revolutionary blueprint for how a city (an Operating System) should be built. It was fast, powerful, and organized.

The Problem: It was "Proprietary." You had to pay a massive amount of money to the "King" (AT&T/Bell Labs) to use the blueprint, and you weren't allowed to see how it was made or change it.

#### 2. GNU: The Freedom Toolset
The Metaphor: The Master Craftsman’s Tools. (Bash (the terminal), GCC (the compiler))
In the 1980s, Richard Stallman wanted to build a city that looked and felt like Unix but was free for everyone to change and share. He started the GNU Project (which stands for "GNU's Not Unix").

What they built: They built the "furniture" and "utilities"—the hammers (compilers), the saws (text editors), and the plumbing (system libraries).

The Missing Piece: They had everything needed for a city except the foundation and the engine (the Kernel).

#### 3. Linux: The Modern Engine
The Metaphor: The People’s Engine.
In 1991, Linus Torvalds built a "Kernel"—the engine that talks directly to the hardware (the SSDs, RAM, and CPUs we discussed). He made it open-source so anyone could help improve it

| Feature | Original Unix | Linux (Ubuntu, RHEL, etc.) | macOS |
| :--- | :--- | :--- | :--- |
| **Origin** | Bell Labs (1970s) | Built from scratch (1991) | Derived from BSD Unix |
| **Cost** | Very Expensive | **Free / Open Source** | Price of the Mac |
| **Code Style** | Proprietary (Closed) | **Open Source (Shareable)** | Partly Open, Partly Closed |
| **Official Name** | **UNIX** | **Unix-like** | **UNIX** |

## 2. Computing Devices and Peripherals

#### HP EliteBook 840 G6.
![image](https://hackmd.io/_uploads/r1KfJZzdWg.png)


#### How much RAM installed ?
16 GB
a very large, "executive-sized" desk. This means you can have multiple applications, dozens of browser tabs, and heavy spreadsheets open all at the same time without your computer slowing down or forcing you to put things away. For modern computing, 16 GB is the sweet spot for excellent multitasking.

<font color="#FF0000">Strong CPU and 16 GB and more RAM is essential for processing large datasets(In-Memory" Rules)</font>
- The "In-Memory" Rule: For a CPU to work on data, that data must be moved from the "Pantry" (Hard Drive) to the "Countertop" (RAM).
- RAM error symptoms: Screen or computer freezes or stops working / blue screen / beeps

![image](https://hackmd.io/_uploads/ryv50lQdWg.png)

#### Which Processor?
(Intel Core i5-8365U)
Multitasking: It has 4 cores and 8 threads. This is like having a worker with eight hands who can juggle multiple assignments at once without dropping anything.

Speed: Its base operating speed is 1.60 GHz, but it can boost up to 4.1 GHz when depending on the workload. This is like a worker who maintains a steady walking pace but can sprint when you need to load a heavy program quickly.
![image](https://hackmd.io/_uploads/SkQ3al7_Wg.png)

#### How much storage?
477 GB
: You can easily fit your daily groceries, your golf clubs, and a few suitcases in here (thousands of documents, PDFs, photos, and standard software). However, because it's a sedan and not a moving van, you couldn't use it to move an entire house in one trip. (Meaning: You wouldn't want to store massive, raw 4K video files or giant video game libraries on it without buying an external drive).

![image](https://hackmd.io/_uploads/BkzjkWG_Zl.png)
####  Which windows operating system?
Windows 11 Pro
he "Pro" (Professional) version means your office has upgraded security features, like BitLocker disk encryption. It also includes tools designed specifically for a business environment, making it safer and easier to connect to corporate networks.

#### When the mouse installed?
![image](https://hackmd.io/_uploads/SkdAHWMO-l.png)

### Disk Manager: Check disk error 
- create and format harddisk partition
![image](https://hackmd.io/_uploads/HJZW2-M_-e.png)

- The disk drives can be shared with others in the same network
- The hardware details give the manufacturer, serial number, and capacity details. 

### What does it mean by Formatting a new hard drive?



**The Metaphor: The Giant, Empty Metal Box**
When you buy a brand-new hard drive and plug it in, your computer’s Operating System (the Office Manager) looks at it and gets confused.

Why? Because an unformatted hard drive is just a massive, empty metal box. There are no drawers, no hanging rails, no green folders, and no labels. If the Office Worker (the CPU) tried to put a document inside, they would just be throwing loose papers into a giant, unorganized pile. They’d never be able to find that document again.
**What "Formatting" Actually Does**
![image](https://hackmd.io/_uploads/Sy91PqzOWe.png)
1. Building the Drawers (Sectors and Tracks)
2.  Choosing the Filing System (File System-NTFS/windows, APFS/Apples, exFAT/universal)
3.  Creating the Master Index (The Master File Table)

**What if you format an Old Hard Drive?**
Make the entire filing cabinet, dump all the old papers into the incinerator, and put in brand new, empty folders." Formatting wipes the slate completely clean. It destroys the old "Master Index," making the old files invisible and allowing the computer to write new data right over the top of them.

## 3. Interfaces and Connectors
- Connectors- Universal Serial Bus
    - 1996: Type A/B mini A/B, 1.5-12 Mbits/sec
    - 2001: Micro A/B 480 Mbits/sec
    - 2008: USB3 - 5 Gbits/sec
    - 2014: TypeC - 10 Gbits/sec
    - 2017: USB 3.2- 20 Gbit/sec
    - 2019: USB 4 - 40 Gbits/sec
![image](https://hackmd.io/_uploads/SJllFqMu-x.png)


- Display System
    - Resolution: How many pixels on the monitor
    - Bit depth: How many numbers of color supported

### GPU
- Types
    - Integrated GPU- Intel's integrated graphics, AMD's APU series
    - Dedicated GPUs- NVDIA GeForce Series, AMD Radeon series
- core components
    - GPU cores
    - VRAM (resolution rendering)
    - Memory Interface (performance)

### Wireless Connection:
- Wired (Ethernet) : Cat6/ Cat8 / Industrial cables - 10 / 40 / 100 Gbps
- wireless (Wi-Fi): Wi-Fi 6 and 7 boast "theoretical" speeds of 9.6 Gbps to 46 Gbp (Interference: wall, distance)




---

#### Match Devices and Connectors

* **Connects peripherals by daisy chaining:** Thunderbolt
* **Connects cameras with computers:** USA-A
* **Connects devices to HDTV:** Mini display port
* **Connects keyboards to gaming consoles:** PS/2

---

#### Disk Configurations Comparison

| Hard Drive | No. of Partitions | Max Volume Size | Max Partition Size | Max Directories | Dir Char Limit | Max File Size | Max No. of Files | File Name Char Limit |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **FAT32** | 32 GB limit / 4 | 2 TB (16 TB for 4 KB sectors) | 32 GB | 65,536 files in a directory | 255 | 4 GB | 268,173,300 | 255 |
| **NTFS** (Windows) | Practical limit is 4 | 8 petabytes | Cluster size determines partition size | No fixed limit | 255 | 16 exabytes | 4,294,967,295 | 255 |
| **HFS+** (Mac) | 2^32 blocks on a volume | Slightly less than 8 EB | 2^32 allocation blocks on volume | Limit based on disk cache | 255 | Slightly less than 8 exabytes | 65,535 | 255 |
| **EXT 4** (Linux) | 4 | 1 EB | 16 TB file / 1 EB volume + 4096 block | Unlimited | 255 / Max path 4096 | 16 Tebibytes | 4,000,000,000 | 255 |
| **HPFS** | 4 | 64 GiB | --- | --- | --- | 2 GiB | Unlimited | 255 |

## 4. Internal Computer Components

### Memories
![image](https://hackmd.io/_uploads/rJPRHGQ_bl.png)

![image](https://hackmd.io/_uploads/rkGkIM7dZe.png)

### **Dynamic Memory Type Comparison Table**
- RAM (Random Access Memory) is your Countertop. It's where you put the ingredients you are actively chopping and cooking right now.

- HDD (Hard Disk Drive) and SSD (Solid State Drive) are your Pantry and Refrigerator. This is where you store all your ingredients for the long term, even when the kitchen is closed and the lights are off.

| Memory Type | Full Name | Primary Optimization | Typical Use Case | Bandwidth & Performance Profile | Physical Form Factor |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Standard DDR** (e.g., DDR4, DDR5) | Double Data Rate SDRAM | **Capacity & Cost-efficiency.** Built to provide large, affordable workspaces. | Desktop PCs, standard enterprise servers, traditional workstations. | **Moderate Bandwidth.** Prioritizes low latency for sequential CPU tasks over massive parallel data transfers. | Long, removable memory sticks (DIMMs) slotted into a motherboard. |
| **LPDDR** (e.g., LPDDR5X) | Low Power Double Data Rate | **Power Efficiency & Space.** Built to maximize battery life while maintaining good speed. | Smartphones, tablets, ultra-thin laptops (like the ThinkPad X13), Edge AI devices. | **Moderate-High Bandwidth.** Uses lower voltages and shorter physical traces to save power. | Chips soldered directly onto the motherboard close to the CPU (no removable sticks). |
| **GDDR** (e.g., GDDR6) | Graphics Double Data Rate | **High Bandwidth.** Built to push massive amounts of visual data or parallel calculations simultaneously. | Consumer graphics cards (NVIDIA GeForce, AMD Radeon), gaming consoles (PS5, Xbox). | **High Bandwidth.** Sacrifices a little bit of latency to achieve massive data throughput for GPU parallel processing. | Memory chips soldered directly onto the graphics card, surrounding the main GPU die. |
| **HBM** (e.g., HBM3, HBM3e) | High Bandwidth Memory | **Extreme Bandwidth & Footprint.** Built to feed data-starved AI processors at the absolute physical speed limit. | Enterprise AI accelerators (NVIDIA H100, AMD MI300), supercomputers, high-end data center GPUs. | **Extreme Bandwidth.** Moves terabytes of data per second using thousands of incredibly wide data channels. | 3D-stacked chips placed on a silicon "interposer" directly next to the GPU (within the same package). |


* The Motherboard: This is the City Map or the ground everything is built on. It’s the main printed circuit board that connects all the "buildings" (components) together.

* The Northbridge: Think of this as the Expressway Entrance right next to the "Mayor's Office" (the CPU). It handles the fastest traffic, like the Graphics Card and Memory.

* The Southbridge: This is the Local Streets manager. It handles the slower stuff, like USB ports and older hard drives, further away from the CPU.


* The Modem: This is the Translator at the city gates. It takes the "foreign language" coming from your ISP (via cable or phone lines) and converts it into the "Digital English" your computer speaks.






* The Router: This is the Traffic Cop inside your house that tells the data which device (phone, laptop, TV) to go to.

#### Storage Devices Comparison

| Type | Capacity | Speeds | Notable Facts |
| :--- | :--- | :--- | :--- |
| **Hard disk drive (traditional HDD)** | 16 GB to 20 TB | 0.1 to 1.7 MB/s. 5,400 RPM to 10,000 RPM, Most spin at 7,200 RPM | Slower than SSD |
| **Solid state disk drives (SSD)** | 120GB to 30.72TB | 600 MB/s. No spinning | Faster speeds |
| **Portable flash memory** | 8 GB to 1 TB | Slower than SSD, Speed based on the port and cable connection | Includes SD cards, USB drives and external SSDs |
| **Hybrid SSD/Flash/HDD** | 20 TB | Still being evaluated | Some include "system on a chip" processing |

---

### **Key Takeaways**
* **Hard Disk Drive :**  Uses mechanical spinning platters (RPM) and a physical "needle" (read/write head). If it’s not under the needle, you have to wait for it to spin around.
* **Solid State Drive:** (The Flash Drive on Steroids): No moving parts. It uses non-volatile flash memory. Uses flash-based memory with no moving parts, resulting in significantly higher speeds (600 MB/s).
* **Capacity:** HDDs and SSDs now offer comparable high-end capacities (up to ~20-30 TB).
* **Portability:** Flash memory (SD cards/USB) is convenient but generally slower than internal SSDs.
### 4.1 Key Concepts: Drive vs. Driver


> **Crucial Distinction:** Do not confuse physical storage with software instructions.

| Term | Type | Definition | Example from System |
| :--- | :--- | :--- | :--- |
| **Drive** | **Hardware** | Physical storage (The "Filing Cabinet"). | **SSD** (Solid State Drive), represented as **C:** |
| **Driver** | **Software** | The instruction manual that tells Windows how to talk to hardware. | **monitor.sys** |

---

### 4.2 The Display System
*Understanding the relationship between the "Artist" and the "Canvas".*

#### A. The Canvas: The Monitor
* **Hardware:** **Integrated Monitor** (Screen built directly into the laptop body).
* **Driver:** Standard Microsoft driver.
    * **File:** `monitor.sys` (Simple instruction file).
    * **Note:** The date is often listed as **2006** (Generic placeholder) to ensure manufacturer drivers take priority.

![Monitor Driver Details](https://hackmd.io/_uploads/BJASsZUU-g.png)
*(Image: Viewing the generic driver file monitor.sys)*

#### B. The Artist: Display Adapter (Graphics Card)
* **Hardware:** **Intel(R) UHD Graphics 620**.
    * **Definition:** An **Adapter** is a hardware translator. It adapts the internal language of the computer (CPU) to the external language of the monitor.
    * **Function:** The monitor doesn't "think"; this Intel chip creates the image, and the monitor simply displays it.
* **Driver:** Specific Intel Manufacturer Driver.
    * **Files:** Complex libraries (e.g., `intel_gfx_api-x64.dll`) that handle 3D graphics and HD video processing.

![Intel UHD Graphics Properties](https://hackmd.io/_uploads/HyfDpb8UWl.png)
![Graphics Driver Files](https://hackmd.io/_uploads/BkHK0ZU8-e.png)

---
## 5. Evaluating Computer Performance and Storage

- Components: 
    - The processor's speed
    - The number of Cores
    - The bus types and Speeds
    - THe presence of cache or other onboard memory

## 6. Network Adapters

### 6.1 Case Study: Coffee Shop Wi-Fi
**Scenario:** You are connected to Wi-Fi ("ACupOfCoffee-5G") in a coffee shop. Which item in the list is doing the work?

![Device Manager Network Adapters](https://hackmd.io/_uploads/r1z4LMI8bx.png)

> **Q: Which network adapter am I using?**
> **A: Intel(R) Wireless-AC 9560**

**Breakdown of List:**
1.  **Intel(R) Wireless-AC 9560:** The **Wi-Fi Card** (Active).
2.  **Intel(R) Ethernet Connection:** The **Cable/LAN Port** (Inactive).
3.  **Fortinet / WAN Miniport:** **Virtual Adapters** (Software only, used for VPNs).

### 6.2 Practice
| # | Question | Correct Answer | Logic & Key Takeaways |
| :--- | :--- | :--- | :--- |
| **1** | Which term identifies the main printed circuit board? | **Motherboard** | The central hub that houses the CPU, RAM, and connectors. |
| **2** | Which chipset connects to the CPU for high-performance tasks? | **Northbridge** | Handles high-speed data (RAM/Video). **Southbridge** handles slower I/O (USB/SATA). |
| **3** | What is a key characteristic of a solid state hard drive (SSD)? | **Faster access to data** | No moving parts means nearly instant data retrieval. |
| **4** | Difference between a traditional HDD and an SSD? | **HDDs = Spinning platters; SSDs = Flash memory.** | HDDs are mechanical and slower; SSDs are electronic and durable. |
| **5** | Which statement is true about GPUs? | **Specialized for rendering graphics.** | They parallel-process data to display images or calculate complex models. |
| **6** | A sound card sends a signal to a computer's ________. | **Speakers** | It converts digital bits into analog sound waves for output. |
| **7** | Which card supports data modeling and visualizations? | **Accelerated graphics card** | GPUs are required to render high-resolution 3D or data-heavy visuals. |
| **8** | Which device converts ISP signals into a digital signal? | **The modem** | **Logic:** Modulator-Demodulator translates analog/fiber to digital. NICs just connect to a network. |
| **9** | What method cools components by slowing hardware speed? | **Passive cooling** | **Logic:** Uses thermal throttling (reducing clock speed) to lower heat without power. |
| **10** | Fans and radiators dissipate heat to prevent damage. | **True** | This is **Active Cooling**, using energy to move heat away. |
Problem: How can you find out the driver details for a network adapter? (Hint: Right-click adapter > Properties > Driver Tab > Driver Details)


-  Question 

It's time to look for a replacement hard drive. Which type of drive dominates today's desktop and laptop market? 

1. Parallel Advanced Technology Attachment (PATA) drives (Speed: 133 megabits/second)
2. Solid-State Drives (SSDs, faster speeds,10-12 gigabits/second,capacity: 120 gigabytes to 2 terabytes, more expensive than SATA  ) 
3. Serial Advanced Technology Attachment (SATA) drives ('serial': data transmission on bit at a time, 6 gigabits/second, spin in 5400-7200 revolution per minute, capacity: 250 gigabytes to 30 terabytes)
4. Small Computer System Interface (SCSI) hard drives (obsolete,spin in 10,000 revolution per minute )
![image](https://hackmd.io/_uploads/SkiVjsZ_-g.png)

 





## 6. Summaries
Even the most complicated machine can be reduced to its basic parts.  Understanding these components can give you an idea of how a computer operates, and this knowledge can allow you to make better decisions when using and servicing your system.  

**-  The Modern Frontier: Hardware Limits in AI**
Understanding these fundamentals is critical for modern computing, specifically in AI. For example, in Retrieval-Augmented Generation (RAG) systems, vector databases frequently exceed available RAM. When the system is forced to page these massive datasets back to the "Pantry," traditional storage bottlenecks the entire pipeline. This is why High IOPS SSDs are now strictly required—to ensure the CPU/GPU is never starved for data while searching through massive information vectors.



## 一文看懂記憶體分類：DRAM：DDR、LPDDR、HBM丨NAND：eMMC、UFS、eMCP、uMCP詳細介紹
## [[紀錄一下自己的理解：RAG 系統中為何要開始導入高 IOPS SSD？](https://www.facebook.com/zheng.kai.yuan.735107/posts/pfbid05yasjaHrtGpHHmizpCvqSUEZnjz42Lpt1zdBYsHfYM5NZ9vdxQ68r6fgihRnNr5ml)]

1. RAG 的代價與 DRAM 成本危機
RAG 的核心是向量資料庫（Vector Database），而目前主流的近似最近鄰搜尋（ANNS）演算法是 HNSW。

- HNSW 的天性： 它追求極致的搜尋速度，代價是必須將龐大的圖結構索引（Graph Index）與向量資料全部塞在 DRAM 裡。

- 維度問題： 從 BERT 時代的 768 維到 OpenAI 的 3072 維，資料點在空間中變得越來越複雜。當企業導入 RAG 且內部文件與用戶暫存資料暴增時，DRAM 的耗用量是呈指數級別上升的。伺服器 DRAM 擴充不僅有物理插槽限制，成本更高昂。

2. 演算法的妥協：從 HNSW 轉向 DiskANN
為了解決 DRAM 破產危機，業界必然走向「降本增效」，這就是 DiskANN 這類 SSD-based 演算法崛起的原因。

- 架構拆分： DiskANN 的核心思想是「分層儲存」。將原始向量經過壓縮後的 PQ (Product Quantization) 向量留在 DRAM 裡做初步的快速篩選，而將最佔空間的 Graph Index 存放到單位成本便宜許多的 SSD 中。

- 效益： 就如鎧俠（Kioxia）的數據，DRAM 用量銳減將近 90%，這在資料中心營運上是巨大的成本勝利。

3. 延遲與「Pointer Chasing」
即便成本降了，但傳統 TLC SSD 帶來了新的效能災難：延遲（Latency）。

- Pointer Chasing（指標追逐）的困境： 在圖結構中搜尋時，演算法必須先讀取節點 A，才知道下一個要走去節點 B。這種「非平行、具備強烈先後相依性」的運算，讓 CPU/GPU 只能「乾等」資料從硬碟傳上來。

- 百倍甚至千倍的落差： DRAM 讀取延遲在 0.1 μs（微秒）等級，而一般企業級 TLC SSD 大約在 100 μs 左右。每一次在圖中的跳躍都要經歷這種延遲，會讓 LLM 推理前的檢索時間嚴重拖長。

4. 救星：高 IOPS / 低延遲 SSD 的必然性
為了解決 DiskANN 帶來的 SSD 延遲瓶頸，硬體必須做出改良，高 IOPS/低延遲 SSD 成為剛需。

補充：

- 回歸 SLC（Single-Level Cell）： 傳統 TLC 一個儲存單元塞 3 bits，讀寫時需要反覆確認電壓狀態，速度慢；SLC 一個單元只存 1 bit（非 0 即 1），雖然容量密度低，但讀寫極快、壽命極長。這能將延遲從 100 μs 壓低到 5~10 μs。

- GPU 直連存取（GDS / GPUDirect Storage）： 未來 GPU 將跳過 CPU 與系統 DRAM，直接向 SSD 抓取 Graph Index。如果 SSD IOPS 不夠高、隨機讀取不夠快，這條直連高速公路就會大塞車。
-  重新設計的 Controller： 傳統 SSD 控制器是為了「大檔連續讀寫」或「一般隨機讀寫」最佳化。未來的 AI 專用 SSD 控制器，可能會針對 ANNS 演算法的存取模式（極高併發、極小區塊的隨機讀取）進行硬體級別的最佳化，甚至加入 Computational Storage（運算型儲存）概念，讓控制器直接分擔部分向量距離計算。
