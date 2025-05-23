# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np
original_array = np.array([[1, 2, 3],
                           [4, 5, 6],
                           [7, 8, 9]])

new_column = np.array([20, 50, 80])  # Must have the same number of rows
array_without_second_column = np.delete(original_array, 1, axis=1)
updated_array = np.insert(array_without_second_column, 1, new_column, axis=1)
print("Original Array:")
print(original_array)

print("\nNew Column to Insert:")
print(new_column)

print("\nUpdated Array with Replaced Column:")
print(updated_array)
```
## Output
Original Array:
[[1 2 3]
 [4 5 6]
 [7 8 9]]

New Column to Insert:
[20 50 80]

Updated Array with Replaced Column:
[[ 1 20  3]
 [ 4 50  6]
 [ 7 80  9]]

## Result
Hence deleteed the second column from a given 2D array and inserts a new column at the same position.
