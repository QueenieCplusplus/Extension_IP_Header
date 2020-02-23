# Extension_IP_Header
擴充的 IP 標頭

# IPv6 Header 

          IPv6 Header            |
          Next Header = TCP      |     TCP Header & Data
          Value 6                |

> Header Fields 

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

features:

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








