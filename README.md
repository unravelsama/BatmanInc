# BatmanInc
code, story, and more interests

```python
#python.C1.IO.csv

import csv
import sys
# filename = 'c:\\pythonfile\\test.csv';

filename = 'c:\\pythonfile2\\test007.csv';

f = open(filename, 'wt')
try:
    writer = csv.writer(f)
    # 写入表头
    writer.writerow( ('Title 1', 'Title 2', 'Title 3') )
    # 数据行 100行
    for i in range(30):
        writer.writerow( (i+1, chr(ord('a') + i), '08/%02d/07' % (i+1)) )
finally:
    f.close()

print(open(filename, 'rt').read())

```
