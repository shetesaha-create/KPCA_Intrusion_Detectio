# ROGRAM 1 — RBF Kernel PCA, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 2 — RBF Kernel PCA, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 3 — RBF Kernel PCA, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 4 — Linear Kernel PCA, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 5 — Linear Kernel PCA, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 6 — Linear Kernel PCA, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 7 — Polynomial Kernel PCA, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 8 — Polynomial Kernel PCA, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 9 — Polynomial Kernel PCA, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 10 — Sigmoid Kernel PCA, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 11 — Sigmoid Kernel PCA, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 12 — Sigmoid Kernel PCA, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 13 — Cosine Kernel PCA, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 14 — Cosine Kernel PCA, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```

# PROGRAM 15 — Cosine Kernel PCA, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]# =========================# 2. PREPROCESSING# =========================X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 3. TRAIN TEST SPLIT
```
