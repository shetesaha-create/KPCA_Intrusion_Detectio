## 1. RBF Kernel — Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 2. RBF Kernel — Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 3. RBF Kernel — Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 4. Linear Kernel — Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 5. Linear Kernel — Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 6. Linear Kernel — Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 7. Polynomial Kernel — Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 8. Polynomial Kernel — Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 9. Polynomial Kernel — Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 10. Sigmoid Kernel — Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 11. Sigmoid Kernel — Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 12. Sigmoid Kernel — Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 13. Cosine Kernel — Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 14. Cosine Kernel — Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```

## 15. Cosine Kernel — Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================
```
