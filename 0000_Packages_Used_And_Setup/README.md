## 1. Packages Used
             import numpy as np 
             import pandas as pd
             import seaborn as sns
             import matplotlib.pyplot as plt
             from sklearn.model_selection import train_test_split
             from sklearn.model_selection import KFold
             from sklearn.preprocessing import LabelEncoder
             from imblearn.over_sampling import RandomOverSampler
             from imblearn.under_sampling import RandomUnderSampler
             from sklearn.ensemble import RandomForestClassifier
             from sklearn.metrics import average_precision_score
             from sklearn.metrics import f1_score
             from sklearn.metrics import classification_report
             from sklearn.metrics import confusion_matrix
             import xgboost as xgb
             from sklearn.metrics import plot_roc_curve
             from sklearn.metrics import PrecisionRecallDisplay
             from sklearn.calibration import CalibratedClassifierCV

## 2. Random State
             random_state = 123
