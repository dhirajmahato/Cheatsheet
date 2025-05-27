

| Operation                       | Python Lists / Dicts       | NumPy Arrays (`np.array`)                 | Pandas Series / DataFrame (`pd.Series` / `pd.DataFrame`) |
| ------------------------------- | -------------------------- | ----------------------------------------- | -------------------------------------------------------- |
| **Create Data**                 | `lst = [1, 2, 3]`          | `arr = np.array([1,2,3])`                 | `s = pd.Series([1,2,3])` / `df = pd.DataFrame(...)`      |
| **Add 10 to Each Element**      | `[x + 10 for x in lst]`    | `arr + 10` (vectorized)                   | `s + 10` (vectorized)                                    |
| **Element-wise Multiplication** | `[x*2 for x in lst]`       | `arr * 2`                                 | `s * 2`                                                  |
| **Mean Calculation**            | `sum(lst)/len(lst)`        | `arr.mean()`                              | `s.mean()`                                               |
| **Sum All Elements**            | `sum(lst)`                 | `arr.sum()`                               | `s.sum()`                                                |
| **Filter > 2**                  | `[x for x in lst if x>2]`  | `arr[arr > 2]`                            | `s[s > 2]`                                               |
| **Indexing**                    | `lst[0]`                   | `arr[0]`                                  | `s.iloc[0]` / `s.loc[label]`                             |
| **Slicing**                     | `lst[1:3]`                 | `arr[1:3]`                                | `s.iloc[1:3]` / `s.loc[...]`                             |
| **Multiple Columns**            | `dict of lists`            | `structured array (complex)`              | `pd.DataFrame({'col1': [...], 'col2': [...]})`           |
| **Group by / Aggregation**      | Manual dict logic          | Not directly supported (need custom code) | `df.groupby('col').agg(...)`                             |
| **Missing Data Handling**       | None (must check manually) | Limited (use `np.nan`, `np.isnan()`)      | Built-in (`isna()`, `fillna()`, `dropna()`)              |
| **Reading CSV**                 | `csv.reader()`             | Limited (`np.loadtxt()`)                  | `pd.read_csv()`                                          |
| **Writing CSV**                 | `csv.writer()`             | `np.savetxt()`                            | `df.to_csv()`                                            |
| **Data Alignment**              | Not available              | Not available                             | Automatic in DataFrame / Series                          |
| **Heterogeneous Data**          | ✅ (list of mixed types)    | ❌ (homogeneous dtype)                     | ✅ (DataFrame columns can have different types)           |
| **Shape / Size Attributes**     | `len(lst)`                 | `arr.shape`                               | `df.shape`                                               |
| **Index / Labels**              | No (only position)         | No                                        | Yes (row & column labels)                                |
| **Best For**                    | Small, mixed-type data     | Numeric, homogeneous arrays (math, ML)    | Real-world data tables (CSV, Excel, SQL, etc.)           |
