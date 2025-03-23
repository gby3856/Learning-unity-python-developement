# 📊 CSV Data Read Test - March 22

This test reads a CSV file (`국가별콘텐츠시장통계정보.csv`) and prints out parts of the data to understand how Python's `csv` module handles it.

---

## 🔍 Code

```python
import csv

data_file = '국가별콘텐츠시장통계정보.csv'
data_pointer = open(data_file, 'r', encoding='utf-8')

data_list = []
reader = csv.reader(data_pointer)
for line in reader:
    data_list.append(line)
print(data_list)

for each_line in data_list[0:2]:
    print(each_line)
