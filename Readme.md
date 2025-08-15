# (Open Systems Interconnection) OSI Model

### What is OSI MODEL

OSI এর পূর্ণ অর্থ হচ্ছে Open Systems Interconnection. নেটওয়ার্কে যখন এক ডিভাইস থেকে আরেক ডিভাইসের মধ্যে যোগাযোগ হয়, তখন OSI মডেলের প্রতিটি লেয়ার পার হতে হয়। OSI মডেলে মোট সাত (০৭) টি লেয়ার থাকে এবং তিনটি (০৩) ভাবে বিভক্ত। উপরের তিনটি (০৩) লেয়ারকে বলা হয় সফটওয়্যার লেয়ার, নিচের তিনটি (০৩) লেয়ার কে বলা হয় হার্ডওয়্যার লেয়ার, আর মাঝের লেয়ার কে বলা হয় কোর (Core) লেয়ার। নেটওয়ার্কে আমরা যত অ্যাপ্লিকেশন ব্যবহার করি তার সবই ব্যবহার হয় উপরের তিনটি লেয়ারে (Application), আর নেটওয়ার্কে যত হার্ডওয়্যার (Router, Switch, Firewall) ব্যবহার করা হয়, তার সবই নিচের তিনটি (০৩) লেয়ারে ব্যবহার করা হয়, আর সফটওয়্যার লেয়ার এবং হার্ডওয়্যার লেয়ারের মাঝে ইন্টারফেসিং করে ট্রান্সপোর্ট লেয়ার। এইজন্য ট্রান্সপোর্ট লেয়ারকে Core লেয়ার বলা হয়। নিচে OSI মডেলের লেয়ার গুলার নাম দেয়া হয়েছে।

- Physical Layer
- Data Link Layer
- Network Layer
- Transport Layer
- Session Layer
- Presentation Layer
- Application Layer

---

#### এপ্লিকেশন লেয়ার:

 এটি হলো ওএসআই মডেলের সপ্তম লেয়ার। এপ্লিকেশন লেয়ার ইউজার ইন্টারফেস প্রদান করে এবং নেটওয়ার্ক ডাটা প্রসেস করে।এপ্লিকেশন লেয়ার যে কাজ গুলো করে থাকে রিসোর্স শেয়ারিং, রিমোট ফাইল একসেস, ডিরেক্টরী সার্ভিস ইত্যাদি। এপ্লিকেশন লেয়ারের কিছু প্রটোকল এর পোর্ট এড্রেস দেওয়া হলো

 প্রটোকল এফটিপি টিএফটিপি টেলনেট ডিএইচসিপি ডিএনএস পপ আইম্যাপ এসএমটিপি এইচটিটিপি পোর্ট এড্রেস ২০/২১ ৬৯ ২৩ ৬৭/৬৮ ৫৩ ১১০ ১৪৩ ২৫ ৮০ পোর্ট নাম্বারগুলো মনে রাখার চেষ্টা করতে হবে। কারণ সিসিএনএ পরীক্ষায় সাধারণত এ ধরনের প্রশ্ন থাকে , যেমন এইচটিটিপি এর পোর্ট নাম্বার কত?

<br>

#### প্রেজেন্টেশন লেয়ার:

এই লেয়ার নেটওয়ার্ক সার্ভিসের জন্য ডাটা ট্রান্সলেটর হিসেবে কাজ করে। এই লেয়ার যে কাজ গুলো করে থাকে ডাটা কনভার্শন,ডাটা কমপ্রেশন, ডিক্রিপশন ইত্যাদি। এই লেয়ারে ব্যবহিত ডাটা ফরম্যাট গুলো হলো .জেপিজি, .এমপিইজি ইত্যাদি।

<br>

#### সেশন লেয়ার:

সেশন লেয়ারের কাজ হলো উৎস এবং গন্তব্য ডিভাইসের মধ্যে সংযোগ গড়ে তোলা , সেই সংযোগ কন্ট্রোল করে এবং প্রয়োজন শেষে সংযোগ বিচ্ছিন্ন করা। ডাটা পাঠানোর জন্য ৩ ধরনের কন্ট্রোল ব্যবহার করা হয় ।

সিম্পলেক্স : সিম্পলেক্স এ ডাটা একদিকে প্রবাহিত হয়। হাফ ডুপ্লেক্স : হাফ ডুপ্লেক্স পদ্ধতিতে একদিকের ডাটা প্রবাহ শেষ হলে অন্যদিকের ডাটা অন্য দিকের ডাটা প্রবাহিত হয়ে থাকে। ফুল ডুপ্লেক্স : ফুল ডুপ্লেক্স পদ্ধতিতে একইসাথে উভয়দিকে ডাটা প্রবাহিত হতে পারে।

<br>

#### ট্রান্সপোর্ট লেয়ার:

ওএসআই মডেলের চতুর্থ লেয়ার ট্রান্সপোর্ট লেয়ার । এই লেয়ারের কাজ হলো সেশন লেয়ারের কাছ থেকে পাওয়া পাওয়া ডাটা নির্ভরযোগ্যভাবে অন্য ডিভাইসে পৌছানো নিশ্চিত করে। এই লেয়ারে ডাটা পৌছানোর জন্য দু’ধরনের ট্রান্সমিশন ব্যবহার করে:

**কানেকশন ওরিয়েন্টেড:**
কানেকশন ওরিয়েন্টেড এ ডাটা পাঠানোর আগে প্রেরক গ্রাহক এর সাথে একটি একুনলেজ সিগন্যাল এর মাধ্যাম কানেকশন তৈরি করে থাকে। ইহা টিসিটি এর ক্ষেত্রে ঘটে থাকে।


**কানেকশনলেস:**
কানেকশনলেস ওরিয়েন্টেড এ ডাটা পাঠানোর আগে প্রেরক গ্রাহক এর সাথে কোন একুনলেজ সিগন্যাল এর মাধ্যাম কানেকশন তৈরি করে থাকে না। ইহা ইউডিপি এর ক্ষেত্রে ঘটে থাকে।

<br>

#### নেটওয়ার্ক লেয়ার :

নেটওয়ার্ক লেয়ারের কাজ হলো এড্রেসিং ও প্যাকেট ডেলিভারি। এই লেয়ারে ডাটা প্যাকেটে নেটওয়ার্ক এড্রেস যোগ করে এনক্যাপসুলেশনের মাধ্যমে। এই লেয়ারে রাউটার ব্যবহিত হয়ে থাকে এবং রাউটিং টেবিল তৈরি করে থাকে।

---
### ফিজিক্যাল লেয়ার :

ফিজিক্যাল লেয়ার OSI Model এর প্রথম লেয়ার যেটি কিনা, সর্বনিম্নে অবস্থান করে। এর নাম থেকে, আপনি আন্দাজ করতে পারেন, এই লেয়ার কি কাজ করে। এই লেয়ার দুটি ফিজিক্যাল ডিভাইস এর মধ্যে সম্পর্ক স্থাপন করে। এবং ফিজিক্যাল কানেকশণ (কোন ক্যাবল এর সাহায্যে) এর সাহায্যে ডাটা এক ডিভাইস থেকে অন্য ডিভাইসে প্রেরণ করা হয়। এই লেয়ার ডাটাকে বিট স্ট্রিমে রুপান্তর করে থাকে অর্থাৎ ডাটাকে 0 এবং 1 এ .রুপান্তর করে থাকে। ডাটাকে বিট টু বিট আকারে ট্রান্সফার করা হয়ে থাকে।

**এই লেয়ারে ব্যবহৃত ডিভাইস গুলো হলোঃ**

- হাব (Hub)
- রাউটার (Router)
- রিপিটার (Repeater)
- নেটওয়ার্ক ক্যাবল (Network Cables)
- মডেম (Modem)
-  NIC (Network Interface Card)

অনেক সময় একটি প্রশ্ন আসে এপ্লিকেশন লেয়ার অথবা নেটওয়ার্ক লেয়ার OSI model এর কততম লেয়ার সহজেই মনে রাখার জন্য এই বাক্যটি মনে রাখতে পারেন।

<br>

|ডিভাইস|কাজ|ব্যাখ্যা|
|---|---|---|
|✅ **Hub**|বিট সিগন্যাল পাঠায়|সব ডিভাইসে একই ডেটা পাঠায়|
|✅ **Repeater**|সিগন্যাল পুনর্জাগ্রত করে|দুর্বল হয়ে যাওয়া সিগন্যাল পুনরায় শক্তিশালী করে|
|✅ **Network Cables**|বিট পরিবহন করে|Twisted Pair, Fiber Optic, Coaxial|
|✅ **Modem**|ডিজিটাল ↔ অ্যানালগ রূপান্তর|Analog লাইনে ডেটা পাঠাতে দেয় (ISP)|
|✅ **NIC (Network Interface Card)**|বিট ট্রান্সমিশনে অংশ নেয়|কম্পিউটারকে নেটওয়ার্কে যুক্ত করে|

---
### ফিজিক্যাল লেয়ার এর প্রধান কাজ:

- বিট ট্রান্সমিশন (1s and 0s)
- মিডিয়া টাইপ নির্বাচন (cable, wireless, fiber)
- ভোল্টেজ লেভেল, টাইমিং, এবং ফ্রিকোয়েন্সি নিয়ন্ত্রণ
- হার্ডওয়্যার সংযোগ তৈরি করা

<br>

#### হাবঃ

- এটি একটি সবচেয়ে সাধারণ নেটওয়ার্কিং ডিভাইস।  
- এটি একাধিক কম্পিউটার বা ডিভাইসকে একটি ল্যান (LAN)–এ সংযুক্ত করে।  
- Hub ডেটা পাঠায় _সব ডিভাইসের_ কাছে—যার জন্য এটি কম নিরাপদ এবং ধীর।
- **উদাহরণ:** স্কুলের পুরনো কম্পিউটার ল্যাব

<br>

#### রাউটারঃ

- এটি একাধিক নেটওয়ার্ককে সংযুক্ত করে (যেমন: আপনার বাড়ির Wi-Fi → ইন্টারনেট)।  
- রাউটার IP address ব্যবহার করে ডেটা রুট করে।  
- এটি Public এবং Private IP address-এর মধ্যে রূপান্তর করে।
- **উদাহরণ:** আপনার বাসার Wi-Fi Router

<br>

#### রিপিটারঃ

- দূরত্ব বাড়লে সিগন্যাল দুর্বল হয়ে যায়—Repeater সেটা পুনরায় শক্তিশালী করে।  
- Signal regeneration করে (1 → 1, 0 → 0)  
- Wired ও Wireless দুটোতেই ব্যবহৃত হয়
- **ব্যবহারঃ**
	- Ethernet cable লাইন যদি 100m এর বেশি হয়
    - Wi-Fi range extender

<br>

#### নেটওয়ার্ক ক্যাবলঃ

- ফিজিক্যালি ডেটা (bit) এক ডিভাইস থেকে আরেকটিতে পাঠায়।
- Twisted Pair (CAT5e, CAT6)
- Coaxial
- Fiber Optic
- **ব্যবহারঃ** 
	- LAN
	- Broadband
	- Data Center

<br>

#### মডেমঃ

- **MO**dulate + **DEM**odulate →  ডিজিটাল ↔ অ্যানালগ সিগন্যাল রূপান্তর করে ইন্টারনেট সংযোগে সহায়তা করে।
- **Physical Layer** (কখনো Data Link এর কিছু অংশও handle করে)
- টেলিফোন লাইন দিয়ে ডেটা ট্রান্সমিটের জন্য দরকার হয়
- **ব্যবহারঃ** 
	- Dial-up
	- DSL
	- Cable Internet

<br>

#### NIC (Network Interface Card):

- কম্পিউটারকে নেটওয়ার্কে যুক্ত করে এবং বিট লেভেলের ডেটা পাঠায়/গ্রহণ করে।
- **Physical + Data Link Layer**  
- MAC Address থাকে  
- Wired বা Wireless NIC হয়
- **ব্যবহারঃ**
	- প্রতিটি কম্পিউটার, ল্যাপটপ বা সার্ভারে একটি NIC থাকে

---
### ক্যাবলিংঃ

#### Twisted Pair Cable (টুইস্টেড পেয়ার ক্যাবল)

- ২ ধরণের হয়:
	- **UTP (Unshielded Twisted Pair)** — সবচেয়ে সাধারণ
    - **STP (Shielded Twisted Pair)** — বেশি ইলেকট্রিক্যাল নিরাপত্তা দেয়

- ব্যবহার:
	- LAN সংযোগ (কম্পিউটার থেকে সুইচ/রাউটার)
	- Ethernet cables (CAT5, CAT6)
	- 

- উদাহরণ:
	- তোমার বাসার রাউটার থেকে ল্যাপটপে যেটা ঢুকানো হয় — সেই **Ethernet Cable**

<br>

#### Coaxial Cable (কোঅক্সিয়াল ক্যাবল)

- গঠন:
	- একটি কপার কোর (core) থাকে, চারপাশে শিল্ডিং এবং ইনসুলেশন
    - সিগন্যাল লস কম হয়
    
- ব্যবহার:
	- পুরাতন কেবল টিভি সংযোগ
    - কিছু ইন্টারনেট কানেকশনে এখনও ব্যবহৃত হয় (DOCSIS modem)

- উদাহরণ:
	- পুরনো দিনে Cable TV বা Broadband সংযোগে

<br>

#### Fiber Optic Cable (ফাইবার অপটিক ক্যাবল)

- গঠন:
	- কাচ বা প্লাস্টিকের তৈরি strand দিয়ে আলোর মাধ্যমে ডেটা ট্রান্সমিশন হয়
    - সবচেয়ে দ্রুত এবং দূরত্ব বেশি কভার করতে পারে
    
- ব্যবহার:
	- ISP বা ডেটা সেন্টার
	- Fast broadband (FTTH – Fiber To The Home)
	 
- উদাহরণ:
	- GP, Banglalink, BDIX–এর অপটিক ফাইবার সংযোগ

<br>

| ক্যাবল টাইপ         | গতি                | দূরত্ব    | দাম    | ব্যবহার                     |
| ------------------- | ------------------ | --------- | ------ | --------------------------- |
| Twisted Pair (CAT6) | 1 Gbps পর্যন্ত     | 100m      | কম     | অফিস, বাসা, LAN             |
| Coaxial             | 10–100 Mbps        | 500m      | মাঝারি | টিভি, পুরাতন নেটওয়ার্ক      |
| Fiber Optic         | 1 Gbps – 100+ Gbps | 10–100 km | বেশি   | ISP, ডেটা সেন্টার, ব্যাকবোন |

---
### X based T Cabling
#### “xBase-T” কী বোঝায়?

| অংশ    | অর্থ                                                               |
| ------ | ------------------------------------------------------------------ |
| `x`    | গতি (Mbps বা Gbps)                                                 |
| `Base` | Baseband transmission (ডেটা একবারে একটি সিগন্যাল হিসেবে পাঠানো হয়) |
| `T`    | Twisted Pair cable (UTP/STP) ব্যবহার করা হয়                        |
<br>

#### Common xBase - T Standards:
| Standard       | গতি      | ক্যাবল টাইপ      | ম্যাক্সিমাম দৈর্ঘ্য |
| -------------- | -------- | ---------------- | ------------------- |
| **10Base-T**   | 10 Mbps  | CAT3 / CAT5 UTP  | 100 মিটার           |
| **100Base-TX** | 100 Mbps | CAT5 UTP         | 100 মিটার           |
| **1000Base-T** | 1 Gbps   | CAT5e/CAT6 UTP   | 100 মিটার           |
| **10GBase-T**  | 10 Gbps  | CAT6a / CAT7 UTP | 100 মিটার           |

<br>

####  ব্যবহার কোথায় হয়?

- **10Base-T** → পুরনো অফিস বা ছোট LAN
- **100Base-TX** → এখনো অনেক জায়গায় ব্যবহার হয় (কম খরচে)
- **1000Base-T** → আজকের দিনে অফিস, বাসা, গিগাবিট রাউটার বা সুইচে
- **10GBase-T** → ডেটা সেন্টার, হাই-স্পিড নেটওয়ার্কিং


**উদাহরণ:**

যদি একটি **Gigabit Switch** আর **CAT6 Ethernet cable** ব্যবহার করো, তাহলে সেটা **1000Base-T** স্ট্যান্ডার্ড অনুযায়ী কাজ করবে।

<br>

### Console Cable কী?

- এটা এমন একটি কেবল যা আপনাকে কম্পিউটারকে সরাসরি একটি রাউটার বা সুইচের **Console Port**-এ সংযুক্ত করতে দেয়।  

- এর মাধ্যমে আপনি **CLI (Command Line Interface)**-এ ঢুকে ডিভাইস কনফিগার করতে পারবেন — ইন্টারনেট ছাড়াই।


#### Console Cable-এর ধরণঃ

- **RJ45 to DB9 Serial Console Cable** (পুরানো)
	- একপাশে RJ45 (Ethernet-এর মতো দেখায়)    
	- অন্যপাশে DB9 Serial Port (COM Port)
	- ব্যবহার হত পুরানো ল্যাপটপ বা ডেস্কটপে

<br>

- **USB to RJ45 Console Cable** (আধুনিক)
	- ল্যাপটপে সিরিয়াল পোর্ট না থাকলে ব্যবহার হয়
    - USB Type-A → RJ45
    - সঙ্গে একটি **USB Serial Driver** (FTDI / Prolific) লাগতে পারে


<br>


|প্রয়োগ|কারণ|
|---|---|
|নতুন সুইচ বা রাউটার কনফিগার|নেটওয়ার্ক পোর্ট কাজ করছে না, সেটআপ দিতে হবে|
|পাসওয়ার্ড রিকভারি|Console access দিয়ে ডিভাইস রিকভারি সম্ভব|
|iOS আপগ্রেড|TFTP দিয়ে ROMmon থেকে ফ্ল্যাশ করা যায়|

<br>

#### **ব্যবহারের ধাপ Cisco রাউটারেঃ**

1. **ক্যাবল সংযুক্ত করুন:**
    - RJ45 end → রাউটারের Console Port   
    - USB end → ল্যাপটপে

2. **Serial/COM Port চেক করুন:**
    - Windows → `Device Manager` → Ports → COMx
    - Linux → `/dev/ttyUSB0` বা `/dev/ttyS0`

3. **Terminal Software চালু করুন:**  
    - [PuTTY](https://www.putty.org)  
    - TeraTerm  
    - Linux-এ `screen /dev/ttyUSB0 9600`

4. **Settings দিন:**    
    - Baud Rate: `9600`
    - Data Bits: `8`
    - Parity: `None`
    - Stop Bits: `1`
    - Flow Control: `None`


<br>

| নাম                                            | মান |
| ---------------------------------------------- | --- |
| 1 **Byte** = 8 **bits**                        |     |
| 1 **Kilobit (Kb)** = 1000 bits (বা 1024 bits)  |     |
| 1 **Kilobyte (KB)** = 1024 bytes = 8192 bits   |     |
| 1 **Megabit (Mb)** = 1000 Kb                   |     |
| 1 **Megabyte (MB)** = 1024 KB = 8,388,608 bits |     |

<br>

#### Bit Rate ক্যালকুলেশনঃ

- **Bit rate** = প্রতি সেকেন্ডে কত বিট পাঠানো হয়
- **উদাহরণঃ**
	- একটি লাইন 10 Mbps স্পিডে কাজ করছে। মানে প্রতি সেকেন্ডে 10,000,000 bits ট্রান্সমিট হয়।

```bash
10 Mbps = 10,000,000 bits/sec = 1.25 MB/sec
```

<br>

#### Transmission Time (TT)

- Transmission Time = (File Size in bits) / (Bandwidth in bps)
- **উদাহরণ:**
	- ধরো 5 MB (Megabyte) ফাইল আছে, আর ব্যান্ডউইথ 10 Mbps।
	-  5 MB = 5 × 8 = **40 Megabits**

```bash
Transmission Time = 40 Mb / 10 Mbps = 4 seconds
```


<br>

#### Baud Rate vs Bit Rate

| নাম           | অর্থ                                     |
| ------------- | ---------------------------------------- |
| **Bit Rate**  | প্রতি সেকেন্ডে কতটি বিট পাঠানো হচ্ছে     |
| **Baud Rate** | প্রতি সেকেন্ডে কতটি সিগনাল পরিবর্তন ঘটছে |

<br>

#### Practical Calculation Example:

- **উদাহরণঃ**
	- A 1 Gbps Ethernet cable transmits data for 2 seconds.
	- How many **bytes** are transmitted?

- Step 1:  
	- 1 Gbps = 1,000,000,000 bits/sec  
	- Time = 2 sec  
	- Total bits = `1,000,000,000 × 2 = 2,000,000,000 bits`

<br>

- Step 2:  
	- Convert bits to bytes:  
	- `2,000,000,000 ÷ 8 = 250,000,000 bytes = 250 MB`
	- **উত্তর: 250 MB**

<br>

#### Encoding Related (NRZ, Manchester)

| Encoding   | Bits per Signal   | Effect on Bit Rate |
| ---------- | ----------------- | ------------------ |
| NRZ        | 1 bit per signal  | Direct mapping     |
| Manchester | 1 bit = 2 signals | Doubles baud rate  |

<br>

#### Physical Layer কীভাবে ফ্রেম ট্রান্সমিট করে?

- Data Link Layer → Frame তৈরি করে
- Physical Layer → Frame কে **bits** (1s and 0s) এ রূপান্তর করে
- Bits → Electrical (copper), Optical (fiber), বা Radio (Wi-Fi) সিগনালে রূপান্তর হয়
- এই সিগনাল কেবল বা তরঙ্গ দিয়ে পৌঁছায় অন্য ডিভাইসে

<br>

#### Frame Transmission Time ক্যালকুলেশন

- Formula:

```bash
Transmission Time = Frame Size (in bits) / Bandwith (in bps)
```

- **Example:**
	- Ethernet Frame Size = 1518 bytes
	- Bandwidth = 100 Mbps

1518 x 8 = 12,144 bits
Time = 12,144 / 100,000,000 = 0.00012144 seconds = 121 µs


<br>

#### VLAN সহ Frame উদাহরণ:

| Dest MAC | Src MAC | VLAN Tag | Type | Payload | FCS |
| -------- | ------- | -------- | ---- | ------- | --- |
| 6 B      | 6 B     | 4 B      | 2 B  | 1500 B  | 4 B |
Frame বড় হলে → More bits → বেশি Transmission Time

---
### ডাটালিংক লেয়ার :

OSI Model এর দ্বিতীয় লেয়ার হলো; ডাটা লিঙ্ক লেয়ার। ডাটা লিঙ্ক লেয়ার অনেকটা নেটওয়ার্ক লেয়ার এর মতো করে ,কাজ করে। নেটওয়ার্ক লেয়ার ডাটা ট্রান্সফার করে থাকে, একই নেটওয়ার্ক এর বাহিরে। কিন্তু ডাটা লিঙ্ক লেয়ার ডাটা প্যাকেট ট্যান্সফার করে থাকে একই নেটওয়ার্ক এর ভিওরে। অথ্যার্ৎ দুটি ডিভাইস যদি, একই নেটওয়ার্ক এর আন্ডারে থাকে ,তাহলে ডাটা লিঙ্ক লেয়ার এর সাহায্যে ডাটা প্যাকেট ট্রান্সমিট করা সম্ভব। ডাটা লিঙ্ক লেয়ার >নেটওয়ার্ক লেয়ার থেকে ডাটা প্যাকেট নেয় এবং ডাটা গুলোকে ছোট ছোট আকারে ভাগ করে, যেটিকে বলা হয় ফ্রেম। নেটওয়ার্ক লেয়ার এর মতোই , এই ডাটা লিঙ্ক লেয়ার , ডাটা প্রবাহ, ডাটা নিয়ন্ত্রন, এরর কন্ট্রোল ইত্যাদি করে থাকে।বলতে পারেন, এই লেয়ার , দুটি ডিভাইসের মধ্যে লজিক্যাল লিঙ্ক তৈরি করে।

<br>

###### কাজঃ

- **বিট → ফ্রেম** এ কনভার্ট করা
- **MAC Address** ব্যবহার করে সরাসরি ডিভাইস চিহ্নিত করা    
- **Error Detection** (Frame-level errors)
- **Flow Control** (যাতে ডেটা অতিরিক্ত না পাঠায়)
- **Media Access Control (MAC)**: কে কবে ডেটা পাঠাবে নির্ধারণ করে

<br>

###### উদাহরণঃ

- কটি পিসি আরেকটি পিসিতে প্যাকেট পাঠাচ্ছে LAN-এর মাধ্যমে
- Data Link Layer সেখানে ডেটা Frame করে   
- MAC address দেখে ফ্রেম ফরওয়ার্ড করে
- শেষে Physical Layer বিট আকারে সেটি পাঠায়

<br>

###### ডাটা লিংক লেয়ার এর দুটি সাব  লেয়ার আছেঃ

- Logical Link Control (LLC): OSI Layer-3 থেকে ফ্রেম গ্রহণ ও পাস করে
- Media Access Control (MAC): ফিজিক্যাল মিডিয়ায় কে কখন ট্রান্সমিট করবে তা নির্ধারণ করে; MAC Address ব্যবহার করে

<br>


**এই লেয়ারে ব্যবহৃত ডিভাইস গুলো হলোঃ**

- সুইচ (Switch)
- ব্রিজ (Bridge)
- NIC (Network Interface Card)


<br>

#### সুইচঃ

- Hub-এর থেকে উন্নত ডিভাইস  
- একটি স্মার্ট ডিভাইস যা **MAC Address Table** ব্যবহার করে  
-  ডেটা নির্দিষ্ট ডিভাইসে পাঠায় (broadcast করে না)
- **Frame Level**-এ কাজ করে
- Collision domain আলাদা করে দেয় প্রতিটি পোর্টের জন্য
- এটি শুধুমাত্র _যার প্রয়োজন_ সেই ডিভাইসে ডেটা পাঠায়।  
- ফাস্টার, বেশি নিরাপদ, এবং নেটওয়ার্কের ট্রাফিক কমায়।
- **ব্যবহার**:
	- LAN
	- Office Network
	- VLAN তৈরি
	
- **উদাহরণঃ**
	- অফিস বা কর্পোরেট LAN যেখানে অনেক কম্পিউটার যুক্ত থাকে
	- PC1 → Switch → PC2 (MAC অনুযায়ী সঠিক পোর্টে ফ্রেম পাঠাবে)

<br>

#### ব্রিজঃ

- দুইটি বা একাধিক নেটওয়ার্ক সেগমেন্টকে সংযুক্ত করে
- Frame Forwarding করে MAC Address দেখে
- খুবই সাধারণ ও সীমিত version of switch
- **ব্যবহারঃ**
	- পুরাতন দিনে LAN-কে ছোট ছোট ভাগে বিভক্ত করতে

- **উদাহরণঃ**
	- LAN1 ↔ Bridge ↔ LAN2

<br>

#### NIC (Network Interface Card):

-  প্রতিটি কম্পিউটারে থাকা কার্ড যা ফ্রেম পাঠায় ও গ্রহণ করে
- MAC Address ধারণ করে (Permanent Layer 2 Address)
- OSI Layer 1+2-তে কাজ করে (Physical + Data Link)
- **ব্যবহার**:
	- কোনো কম্পিউটার নেটওয়ার্কে কানেক্ট করার জন্য অবশ্যই NIC দরকার

- **উদাহরণঃ**
	- Ethernet LAN port বা Wi-Fi card


<br>

| ডিভাইস                         | ব্যাখ্যা                                               |
| ------------------------------ | ------------------------------------------------------ |
| ✅ **Access Point**             | Wi-Fi clients-এর MAC address ধরে ফ্রেম ফরওয়ার্ড করে    |
| ✅ **Layer 2 Switch with VLAN** | VLAN tagging/trunking MAC + VLAN ID দেখে ফ্রেম রুট করে |

| ডিভাইস           | কাজ                            | L2 Role           | আজকের প্রাসঙ্গিকতা |
| ---------------- | ------------------------------ | ----------------- | ------------------ |
| **Switch**       | MAC অনুযায়ী ফ্রেম ফরওয়ার্ড     | ✅ পুরোদমে Layer 2 | ✅ স্ট্যান্ডার্ড    |
| **Bridge**       | দুই LAN সেগমেন্ট যুক্ত করে     | ✅ Simple L2       | ❌ পুরাতন           |
| **NIC**          | MAC address বহন করে            | ✅ L2 + L1         | ✅ অপরিহার্য        |
| **Access Point** | Wi-Fi MAC-based ফ্রেম ডেলিভারি | ✅ আংশিক L2        | ✅ Wireless Network |

<br>

#### **MAC Spoofing** (ম্যাক স্পুফিং)

- MAC spoofing মানে হচ্ছে একটি ডিভাইস ইচ্ছাকৃতভাবে তার আসল **MAC Address পরিবর্তন করে অন্য একটি ভুয়া MAC Address** ব্যবহার করা।

<br>

##### কেন করে?

- Network Bypass (Access Control পাস করতে)
- IP Conflict তৈরি করে নেটওয়ার্কে সমস্যা করা
- অন্য কারো হয়ে আচরণ করা (Impersonation)
- Captive portal হ্যাক করা (Wi-Fi login bypass)
- **উদাহরণঃ**

```bash
sudo ip link set dev eth0 address 00:11:22:33:44:55
```

- **প্রতিরোধ:**
	- Port Security (Cisco switch-এ)
	- DHCP snooping
    - 802.1X authentication

<br>

#### VLAN (Virtual LAN)

- VLAN মানে একই Switch-এর ভেতরে আলাদা আলাদা virtual নেটওয়ার্ক তৈরি করা, যেন তারা আলাদাভাবে আচরণ করে।

<br>

##### কেন করে?

- Security: ডিপার্টমেন্ট বা টিম আলাদা রাখা
- Performance: Broadcast domain ছোট করা
- Network Management সহজ হয়
- **উদাহরণঃ**

```bash
VLAN 10 – HR
VLAN 20 – IT
VLAN 30 – Finance
```

- VLAN 10-এর ইউজার VLAN 20-এ সরাসরি কথা বলতে পারবে না, যতক্ষণ না Routing থাকে।

<br>

#### Trunking

- Trunking মানে একটি লাইন দিয়ে **একাধিক VLAN-এর ফ্রেম** একসাথে পাঠানো। Trunk port VLAN Tag (802.1Q) ব্যবহার করে জানায় কোন VLAN থেকে ফ্রেম এসেছে।

<br>

##### কোথায় দরকার?

- যখন দুইটি VLAN-aware Switch কে যুক্ত করতে হয়
- Switch ↔ Router (Router-on-a-Stick) সংযোগে
- **উদাহরণঃ**

```bash
Switch1 Port Gig0/1 → Trunk Port
Switch2 Port Gig0/1 → Trunk Port
```
- VLAN 10, 20, 30 এর ট্যাগ সহ ফ্রেম যাবে এই লিংকে।

<br>

#### Ethernet Frame Structure

- Ethernet II

> | Preamble | Dest MAC | Src MAC | Type | Payload | FCS |


<br>

| Field                           | Size          | Description                                |
| ------------------------------- | ------------- | ------------------------------------------ |
| **Preamble**                    | 7 bytes       | Start signal for synchronization           |
| **SFD (Start Frame Delimiter)** | 1 byte        | Indicates start of actual frame            |
| **Destination MAC**             | 6 bytes       | কার কাছে যাবে                              |
| **Source MAC**                  | 6 bytes       | কে পাঠাচ্ছে                                |
| **Type/Length**                 | 2 bytes       | উপরের লেয়ারের প্রোটোকল (ex: 0x0800 = IPv4) |
| **Payload**                     | 46–1500 bytes | আসল ডেটা (IP packet ইত্যাদি)               |
| **FCS (CRC)**                   | 4 bytes       | Error checking (CRC)                       |

<br>

#### MAC Address কী ?

- এটি হলো একটি **48-bit (6-byte)** ইউনিক আইডি, যা প্রতিটি NIC (Network Interface Card)-এ থাকে। 
- উদাহরণ: 
	- 00:1A:2B:3C:4D:5E

<br>

#### MAC Address গঠন (Structure)

- MAC Address → **48-bit** → **Hexadecimal format** এ প্রকাশ করা হয়:

```bash
00:1A:2B:3C:4D:5E
```

<br>


| অংশ          | নাম                                          | ব্যাখ্যা                                   |
| ------------ | -------------------------------------------- | ------------------------------------------ |
| 1st 3 Bytes  | **OUI** (Organizationally Unique Identifier) | নির্মাতা কোম্পানির কোড (যেমন Intel, Cisco) |
| Last 3 Bytes | **NIC Specific ID**                          | ইউনিকভাবে ডিভাইস চিহ্নিত করে               |

<br>

#### Binary → Hexadecimal:

- ধরো, একটা MAC address এর binary হচ্ছে:

```bash
00000000 00011010 00101011 00111100 01001101 01011110
```

- এটি 6 টি 8-bit block  
- Hex রূপে: `00:1A:2B:3C:4D:5E`


<br>

#### MAC Address Type Check (Unicast, Multicast, Locally Administered)

- MAC address-এর প্রথম byte থেকেই কিছু তথ্য বোঝা যায়।

```bash
First Byte: 02 → Binary: 00000010
```

| Bit       | অর্থ                                                |
| --------- | --------------------------------------------------- |
| 1st (LSB) | 0 → Unicast, 1 → Multicast                          |
| 2nd       | 0 → Globally Administered, 1 → Locally Administered |

- **উদাহরণ:**

- `00:1A:2B:3C:4D:5E` → Unicast + Globally assigned
- `02:1A:2B:3C:4D:5E` → Unicast + Locally assigned (spoofed address)


<br>

#### Random MAC Generation (for spoofing/testing)

- MAC spoofing বা virtual machine setup-এ MAC address তৈরি করতে হয়।
- MAC Generating Script:

```python
import random

def random_mac():
    mac = [0x02, 0x00, 0x00,
           random.randint(0x00, 0x7f),
           random.randint(0x00, 0xff),
           random.randint(0x00, 0xff)]
    return ':'.join(map(lambda x: "%02x" % x, mac))

print(random_mac())
```

<br>

#### MAC Address Checking Tool

- Windows:

```bash
getmac
ipconfig /all
```

<br>

- Linux:

```bash
ip link show
```

<br>

- Wireshark:

> Filter: `eth.addr == aa:bb:cc:dd:ee:ff`


<br>

#### **Standard Ethernet Frame Structure (Without VLAN)**


| Destination MAC | Source MAC | EtherType | Payload     | Frame Check Sequence |
| --------------- | ---------- | --------- | ----------- | -------------------- |
| (6 bytes)       | (6 bytes)  | (2 bytes) | (46–1500 B) | (FCS – 4 bytes)      |

- **EtherType**: সাধারণত 0x0800 = IPv4, 0x0806 = ARP  
- **FCS**: CRC32 checksum (error checking)


<br>

#### Ethernet Frame with VLAN Tag (IEEE 802.1Q)


| Destination MAC | Source MAC     | Tag   | EtherT | Payload    | FCS   |
| --------------- | -------------- | ----- | ------ | ---------- | ----- |
| (6 bytes)       | (6 bytes)      | (4 B) | (2 B)  | (46–1500B) | (4 B) |
|                 | VLAN Tag Field |       |        |            |       |
<br>

| Bits    | নাম            | কাজ                 |
| ------- | -------------- | ------------------- |
| 3 bits  | PCP (Priority) | QoS (802.1p)        |
| 1 bit   | DEI            | Drop Eligibility    |
| 12 bits | VLAN ID        | 0–4095 পর্যন্ত VLAN |

<br>

#### What is Frame?

- **Frame** হলো Data Link Layer (OSI Layer 2)-এর ইউনিট। এটি IP Packet কে ঘিরে ধরে MAC address, VLAN Tag ইত্যাদি যোগ করে নিচে Physical Layer-এ পাঠায়।
- Frame → Physical Layer-এ গেলে **বিটে রূপান্তর হয়**, এবং কেবল/এয়ার দিয়ে **signal** আকারে ট্রান্সমিট হয়।

<br>

#### Frame → Bits → Signals (Physical Transmission)

| Dest MAC | Src MAC | EtherType | Payload | CRC |
| -------- | ------- | --------- | ------- | --- |
| 6 byters | 6 bytes | 2 bytes   | ~1500 B | 4 B |

- মোট ফ্রেম সাইজ (**without VLAN**):
	- 6 + 6 + 2 + 1500 + 4 = ~1518 bytes (standard max size)

<br>

- এটিকে Physical Layer এ পাঠানো হলে:
	- 1518 bytes × 8 = 12,144 bits
	- এই 12,144 **bits** = **1 Ethernet frame** যা Physical Layer সিগনালে রূপান্তর করে

---
### Broadcast Domain কী?

- একটি Broadcast Domain হলো সেই নেটওয়ার্ক এলাকা যেখানে **একটি ব্রডকাস্ট মেসেজ পাঠালে সেটা সেই এলাকার সব ডিভাইস পায়।**

<br>

-  উদাহরণ:
	- যদি A কম্পিউটার একটা ARP Request পাঠায়:  
	    ➤ "Who has IP 192.168.1.5? Tell 192.168.1.2"  
	    ➤ তাহলে একই Broadcast Domain-এর সব ডিভাইস তা পাবে


<br>

|বৈশিষ্ট্য|ব্যাখ্যা|
|---|---|
|Uses MAC-level Broadcasts|eg. ARP, DHCP|
|Switch বা Hub ভেতরে Same Domain|একে অপরকে Broadcast করে|
|Router → Broadcast Block করে|Router 2টি আলাদা domain তৈরি করে|
|VLAN → আলাদা Broadcast Domain তৈরি করে|VLAN 10 ≠ VLAN 20|

<br>

#### **Collision Domain** কী?

- একটি Collision Domain হলো সেই নেটওয়ার্ক এলাকা যেখানে একাধিক ডিভাইস একই সময়ে ডেটা পাঠালে **collision (ধাক্কা)** লাগে।

<br>

- ### উদাহরণ:

	- যদি A ও B একই সময় ডেটা পাঠায় একটি Hub দিয়ে যুক্ত অবস্থায়, তাদের সিগনাল একে অপরকে ধাক্কা দেবে।


|বৈশিষ্ট্য|ব্যাখ্যা|
|---|---|
|Hub → সব পোর্ট একই collision domain|অর্থাৎ ধাক্কা লাগবে|
|Switch → প্রতিটি পোর্ট আলাদা|collision নেই|
|Full Duplex Mode → No Collision|একসাথে পাঠানো ও পাওয়া যায়|

<br>

##### উদাহরণঃ 

```bash
PC1 ----+
        |
       Hub ------ PC2
        |
       PC3
```

<br>

এখানে Hub ব্যবহার করা হয়েছে, তাই:

- **1 Broadcast Domain**
- **1 Collision Domain** (PC1, 2, 3 → একই সঙ্গে পাঠালে collision হবে)

<br>

##### আরেকটা উদাহরণ Switch দিয়ে:

```bash
PC1 --- Switch --- PC2
        |
       PC3
```

এখানে Switch ব্যবহার করা হয়েছে:

- **1 Broadcast Domain**
- **3 Collision Domain** (প্রতিটি পোর্ট আলাদা)

<br>

#### CSMA / CD - Carrier Sense Multiple Access with Collision Detection

- এটি একটি **network access method**, যা **Ethernet (wired LAN)**-এ ব্যবহৃত হয় — বিশেষ করে পুরোনো দিনে **Hub-based LANs**-এ।

| অংশ                     | অর্থ                                              |
| ----------------------- | ------------------------------------------------- |
| **Carrier Sense**       | লাইন ব্যস্ত কি না, আগে দেখে                       |
| **Multiple Access**     | একাধিক ডিভাইস একসাথে একই মিডিয়া ব্যবহার করতে পারে |
| **Collision Detection** | ধাক্কা লাগলে (collision), তা বুঝতে পারে ও ঠিক করে |

<br>

## CSMA/CD কাজের ধাপ:

- **Carrier Sense:**  
	- ডিভাইস দেখে network line (medium) ফাঁকা কি না

- যদি ফাঁকা হয় → ডেটা পাঠায়  
	- যদি ব্যস্ত হয় → কিছু সময় অপেক্ষা করে আবার চেষ্টা করে

- **Collision হলে:**  
	- দুই ডিভাইস একসাথে ডেটা পাঠালে **Collision** হয়

- **Jam Signal পাঠানো হয়** → সবাইকে জানায় collision হয়েছে

-  **Backoff Time হিসাব করা হয় (random delay)**  
	- Binary Exponential Backoff Algorithm ব্যবহার করে

<br>

#### উদাহরণ (ধাপে ধাপে):

- ধরো PC-A এবং PC-B একই হাব-এ যুক্ত:
	- A লাইন দেখে ফাঁকা, তাই ডেটা পাঠায়
	- B-ও একই সময়ে ফাঁকা দেখে ডেটা পাঠায়
	- তাদের সিগনাল **hub-এ গিয়ে ধাক্কা খায় (collision)**
	- দুইটা ডিভাইস **Jam signal পাঠায়**
	- কিছুক্ষণ অপেক্ষা করে আবার চেষ্টা করে

<br>

| মাধ্যম                    | CSMA/CD                                     |
| ------------------------- | ------------------------------------------- |
| **Ethernet (with Hub)**   | ✅ প্রযোজ্য                                  |
| **Switch-based Ethernet** | ❌ Collision নেই, তাই দরকার নেই              |
| **Wi-Fi (802.11)**        | ❌ CSMA/CA (Collision Avoidance) ব্যবহার করে |

<br>

## Why It’s Obsolete Now?

> ❌ CSMA/CD এখনকার **Switch-based Full Duplex Network**-এ প্রয়োজন নেই কারণ:

- প্রতিটি পোর্ট = আলাদা collision domain
- একই সাথে পাঠানো ও রিসিভ করা যায়
- Collisions ঘটে না

> CSMA/CD = চেষ্টা করো → ধাক্কা লাগলে বুঝো → অপেক্ষা করে আবার পাঠাও


<br>

#### VLAN কী?

- **VLAN (Virtual LAN)** হলো একটি প্রযুক্তি যা **একটি switch-এর ভেতরে বা একাধিক switch-এর মধ্যে** আলাদা আলাদা virtual network তৈরি করে, যেন তারা আলাদা নেটওয়ার্ক হিসেবে কাজ করে।


<br>

##### উদাহরণ:

ধরো একটা কোম্পানিতে ৩টি ডিপার্টমেন্ট:

- HR
- IT
- Finance
    

তাদের সবাই একই switch-এ সংযুক্ত। এখন, তুমি চাও HR-র পিসিগুলো যেন IT বা Finance-এর সাথে কথা না বলে।

<br>

|VLAN ID|ডিপার্টমেন্ট|
|---|---|
|VLAN 10|HR|
|VLAN 20|IT|
|VLAN 30|Finance|

<br>

|Device|Port|VLAN Assigned|
|---|---|---|
|PC1 (HR)|Fa0/1|VLAN 10|
|PC2 (HR)|Fa0/2|VLAN 10|
|PC3 (IT)|Fa0/3|VLAN 20|
|PC4 (Finance)|Fa0/4|VLAN 30|

<br>

#### VLAN Trunking (Multiple VLAN Pass)

যখন দুইটা switch বা router কে VLAN-aware করতে হয়, তখন trunk port ব্যবহার হয়।

- Trunk Port → carries **multiple VLANs** at once
	- VLAN Tagging হয় IEEE 802.1Q দিয়ে  
	- Tag = VLAN ID + Priority info

<br>

##### VLAN Tag Example (Frame Structure):

| Dest Mac | Src MAC | 802.1Q Tag | EtherType | Payload | CRC |
| -------- | ------- | ---------- | --------- | ------- | --- |
| 6 B      | 6 B     | 4 B        | 2 B       | ~1500 B | 4 B |

<br>

##### VLAN Configuration Example (Cisco IOS):

```bash
Switch> enable
Switch# configure terminal
Switch(config)# vlan 10
Switch(config-vlan)# name HR
Switch(config)# interface fa0/1
Switch(config-if)# switchport mode access
Switch(config-if)# switchport access vlan 10
```

<br>

- Trunk Port config:

```bash
Switch(config)# interface fa0/24
Switch(config-if)# switchport mode trunk
Switch(config-if)# switchport trunk allowed vlan 10,20,30
```

<br>

|সুবিধা|ব্যাখ্যা|
|---|---|
|🔐 **Security**|আলাদা ডিপার্টমেন্টকে আলাদা রাখা|
|🚀 **Performance**|Broadcast domain ছোট হয়|
|⚙️ **Flexibility**|একই switch-এ আলাদা নেটওয়ার্ক|
|🧠 **Manageability**|VLAN-based policy enforce সহজ হয়|

|দিক|VLAN|Subnet|
|---|---|---|
|Layer|Layer 2|Layer 3|
|Function|Logical group|IP level separation|
|Need Routing?|VLAN ↔ VLAN → Routing needed|Subnet ↔ Subnet → Routing needed|

---


