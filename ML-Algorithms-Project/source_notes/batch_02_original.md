## Experiment 1 — RBF Kernel, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.2, random_state=0, stratify=y
```

## Experiment 2 — RBF Kernel, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.4, random_state=0, stratify=y
```

## Experiment 3 — RBF Kernel, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.6, random_state=0, stratify=y
```

## Experiment 4 — Linear Kernel, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.2, random_state=0, stratify=y
```

## Experiment 5 — Linear Kernel, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.4, random_state=0, stratify=y
```

## Experiment 6 — Linear Kernel, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.6, random_state=0, stratify=y
```

## Experiment 7 — Polynomial Kernel, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.2, random_state=0, stratify=y
```

## Experiment 8 — Polynomial Kernel, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.4, random_state=0, stratify=y
```

## Experiment 9 — Polynomial Kernel, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.6, random_state=0, stratify=y
```

## Experiment 10 — Sigmoid Kernel, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.2, random_state=0, stratify=y
```

## Experiment 11 — Sigmoid Kernel, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.4, random_state=0, stratify=y
```

## Experiment 12 — Sigmoid Kernel, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.6, random_state=0, stratify=y
```

## Experiment 13 — Cosine Kernel, Test Size 0.2

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.2, random_state=0, stratify=y
```

## Experiment 14 — Cosine Kernel, Test Size 0.4

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.4, random_state=0, stratify=y
```

## Experiment 15 — Cosine Kernel, Test Size 0.6

```
import numpy as npimport pandas as pd# =========================# 1. LOAD DATA# =========================df1 = pd.read_csv('Tuesday-WorkingHours.pcap_ISCX.csv', low_memory=True)df2 = pd.read_csv('Wednesday-workingHours.pcap_ISCX.csv', low_memory=True)df3 = pd.read_csv('Thursday-WorkingHours-Morning-WebAttacks.pcap_ISCX.csv', low_memory=True)dataset = pd.concat([df1, df2, df3], ignore_index=True)dataset.columns = dataset.columns.str.strip()X = dataset.iloc[:, :-1]y = dataset.iloc[:, -1]X = X.apply(pd.to_numeric, errors='coerce')X.replace([np.inf, -np.inf], np.nan, inplace=True)from sklearn.impute import SimpleImputerimputer = SimpleImputer(strategy='mean')X = imputer.fit_transform(X)from sklearn.preprocessing import LabelEncoderlabelencoder_y = LabelEncoder()y = labelencoder_y.fit_transform(y)# =========================# 2. SPLIT DATA# =========================from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X, y, test_size=0.6, random_state=0, stratify=y
```
