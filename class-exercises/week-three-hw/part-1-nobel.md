## Worked with Steven Chau

# 1 

<cut -d "," -f 3 nobel.csv | sort -d | tail -n +2 | grep -w "chemistry" | wc -l> 
## 181

<cut -d "," -f 3 nobel.csv | sort -d | tail -n +2 | grep -w "economics" | wc -l> 
## 81

<cut -d "," -f 3 nobel.csv | sort -d | tail -n +2 | grep -w "literature" | wc -l> 
## 114

<cut -d "," -f 3 nobel.csv | sort -d | tail -n +2 | grep -w "medicine" | wc -l> 
## 216

<cut -d "," -f 3 nobel.csv | sort -d | tail -n +2 | grep -w "peace" | wc -l> 
## 133

<cut -d "," -f 3 nobel.csv | sort -d | tail -n +2 | grep -w "physics" | wc -l> 
## 210

# 2

<cut -d "," -f 5-6 nobel.csv | sort -d | uniq -d>
## Comité international de la Croix Rouge (International Committee of the Red Cross)
## Federick Sanger
## John Bardeen
## Linus Carl Pauling
## Marie Curie
## Office of the United Nations High Commissioner for Refugees (UNHCR)

# 3

<cut -d "," -f 6 nobel.csv | sort -d | uniq -c | sort -n | tail -n 5>
## Smith (5 occurances)
## Wilson (4 occurances)
## Fischer (4 occurances)

# 4

<cut -d "," -f 3 nobel.csv | sort -d | uniq -c | sort -n | tail -n 1>
## Medicine (216 occurances)

<cut -d "," -f 3 nobel.csv | sort -d | uniq -c | sort -n | head -n 2 | tail -n +2>
## Economics (81 occurances)
