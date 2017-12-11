# Sniffer

Simple sniffer using scapy and wxpthon.

## Getting Started

Just download them all and run main.py

### Prerequisites

Use modified [scapy3k](https://github.com/phaethon/scapy)

Only test and modify the lib concerning Windows users.

Need to install [Win10Pcap(Recommended)](http://www.win10pcap.org/), Npcap(might have slight issue of missing certain packets).

### Usage
```
python main.py
```

## Feature

Multiple features in this project.

### Filter on Network interfaces, Protocol, Src, Dst, Sport and Dport.

Choose the filter anytime you like and then click the start button twice to continue sniffering.(have to stop and start to take effect)

### Save selected packet(s) information to files.

Select one packet, or use Ctrl+LeftClick to choose multiple packets. You can save them into a txt file with readable format.

### TCP/IP/HTTP reassembly and save them to files.

Select one packet, and it will automatically find related packets and reassemble them.
After that processing, you are welcome to click the `Reassembly` button to convert them into one entire file.
Only tested in FTP Transmission, HTML reassembly and ICMP(ping), and the file size can be up to 15MB (might take certain time processing to GUI)

### Search bar makes things easier

Using search bar wisely can actually save a lot of time.
Keywords are searched in whole packet's hex or decoded by UTF-8 and GB2312,which is very convenient to find http headers of filename.

### MAX Module

The default MAX module will never let you down when an additional dedicated process is used for listening and sniffering.
However, it is very CPU-consuming, but you can turn it off any time (have to stop and start to take effect)

### Network Speed

Although the value might be lower than the actual one due to the bottleneck of loading and computation, it's better than nothing!

## Sample

![Sample](/sample.png "Sample"){:height="50%" width="50%"}