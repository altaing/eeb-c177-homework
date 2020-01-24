## Workded with Steven Chau

#1

<cut -d "," -f 10 European_Red_List.csv | tail -n +2 | sort -d | uniq -c>
## 456 CR
## 8 CR (PE)
## 2409 DD
## 687 EN
## 4 EW
## 29 EX
## 5805 LC
## 411 NA
## 4 NE
## 964 NT
## 8 RE
## 885 VU

#2

<cut -d "," -f 4,10 European_Red_List.csv | tail -n +2 | sort -d | grep -w "AVES" | uniq -c>
## 10 AVES,CR
## 18 AVES,EN
## 2 AVES,EX
## 428 AVES,LC
## 32 AVES,NT
## 4 AVES,RE
## 39 AVES,VU

#3

<cut -d "," -f 4,10 European_Red_List.csv | tail -n +2 | sort -d | grep -w "AVES" | grep -w 'EX\|RE\|CR' | uniq -c>
## 10 AVES,CR
## 2 AVES,EX
## 4 AVES,RE


