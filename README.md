# Extension_IP_Header
擴充的 IP 標頭

Preface for Basic Network

see <https://github.com/QueenieCplusplus/Networking>

![header](https://static.thegeekstuff.com/wp-content/uploads/2012/03/ip-header-1.png)

# IPv6 Header 

![ipv6](https://blog-imgs-78-origin.fc2.com/h/a/n/hanteye01/2015041016563768c.png)

> Header looks like

          IPv6 Header            |
          Next Header = TCP      |     TCP Header & Data
          Value 6                |

> Header Fields & holding space

![ipv6 header](https://blog-imgs-78-origin.fc2.com/h/a/n/hanteye01/20150410170156c43.png)

        Version 6

        Traffic Class (Procendence)

        Flow Label (to make flag on sequence)

        Payload Length

        Next Header (the extension header, the topic we discuss hereby)

        Hop Limit, 中繼

        Src Addr

        Des Addr
        
> Drop Header, return

        A Msg shows ICMPv6 Param Problem

# Extension Header

![extension](https://blog-imgs-78-origin.fc2.com/h/a/n/hanteye01/201504101705496c8.png)

* Encapsulation Sec Payload Header

* Auth Header

* Routing Header

        有欄位稱為 Segemt Left, 能顯示還有多少節點需要拜訪

* Hop-by-Hop Options Header

# AH, Auth Header

> AH Fileds

* Next Header = Auth Header

* Reserverd 

* SPI, Security Param Index

* Payload Data

* Seq num

* Checksum

# ESP, Encapsulation Security Payload Header

> Features:

(1) anti-replay

(2) auth

(3) confidence

(4) integrity

> ESP Fields

* SPI

* Payload Data (Encypted Data)

* Seq num

* Next Header = Auth Header

* Auth Data

# Combination of Auth & ESP

![combine](https://blog-imgs-78-origin.fc2.com/h/a/n/hanteye01/2015041017115864d.png)

(talk later)

# Tech for Trans/Rcv

* 4 & 6 Dual Stack

* Tunneling

  <https://www.wikiwand.com/en/Layer_2_Tunneling_Protocol>

* 4To6

(to be continued...)

# Tunneling

![tunnel](https://upload.wikimedia.org/wikipedia/en/9/9a/L2tp_pkt_exchg.PNG)

