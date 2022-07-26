# Imputer
Rumming imputer code snippet takes 60 to 90 minutes. So I saved the imputed files and imputer model so that I can save time when I re-run the code.

Putting `knn_imputing = True` will apply KNN imputer while `knn_imputing = False` will just use the saved file.
ruby```
knn_imputing = False
target='site_eui'
#train_dataset.csv
if knn_imputing:
    imputer = KNNImputer(n_neighbors=7)
    tmp = df_all[['State_Factor', 'building_class', 'facility_type', 'dataset', target]]
    df = df_all.drop(tmp.columns, axis=1)
    df1 = pd.DataFrame(imputer.fit_transform(df),columns = df.columns)
    
    tmp.to_csv('/content/imputer_tmp.csv', index=False)
    df1.to_csv('/content/imputer_df1.csv', index=False)
    joblib.dump(imputer, 'models/knn_imputer.pkl')

else:
    df1 = pd.read_csv('/content/imputer_df1.csv')
    tmp = df_all[['State_Factor', 'building_class', 'facility_type', 'dataset', target]]
    df_all = df_all.drop(tmp.columns, axis=1)
    
    for col in tmp.columns:
        df_all[col]=tmp[col]
    for col in df1.columns:
        df_all[col] = df1[col]
```
