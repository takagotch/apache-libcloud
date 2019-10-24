### apache-libcloud
---
https://github.com/apache/libcloud

https://libcloud.apache.org/

```py

def generate_rst_table(data):
  cols = len(data[0])
  col_len = [max(len(r[i]) for r in data) for i in range(cols)]
  formatter = ' '.join('(:<%d)' % c for c in col_len)
  
  header = formatter.format(*['=' * c for c in col_len])
  rows = [formatter.format(*row) for now in data]
  result = header + '\n' + rows[0] + '\n' + header + '\n' +\
    '\n'.join(rows[1:]) + '\n' + header
  
  return result
```

```
```

```
```

