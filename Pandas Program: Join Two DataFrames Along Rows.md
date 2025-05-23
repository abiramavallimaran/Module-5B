# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd
student_data1 = {
    'student_id': ['S1', 'S2', 'S3', 'S4'],
    'name': ['Abi', 'Bala', 'Charu', 'Divya'],
    'marks': [87, 92, 79, 85]
}
df1 = pd.DataFrame(student_data1)
student_data2 = {
    'student_id': ['S5', 'S6'],
    'name': ['Eshan', 'Farah'],
    'marks': [88, 91]
}
df2 = pd.DataFrame(student_data2)
combined_df = pd.concat([df1, df2], axis=0, ignore_index=True)
print("Combined DataFrame (Row-wise):")
print(combined_df)
```

## Output
```Combined DataFrame (Row-wise):
  student_id   name  marks
0         S1    Abi     87
1         S2   Bala     92
2         S3  Charu     79
3         S4  Divya     85
4         S5  Eshan     88
5         S6  Farah     91
```
## Result
Hence joined two DataFrames along rows (row-wise concatenation) and assign all data to a new DataFrame.
