import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df = pd.read_csv (r'K1.csv')
print(df.head(3))
df1 = df[['Distance', 'Direction','DNA Conc.']]
print(df1.head())
heatmap1_data = pd.pivot_table(df1, values='DNA Conc.',index=['Distance'],columns='Direction')
sns.heatmap(heatmap1_data, cmap="YlGnBu")
plt.show()
df2 = df[['Time','Distance', 'Direction','DNA Conc.']]
heatmap2_data = pd.pivot_table(df2,values='DNA Conc.', index=['Time'], columns='Direction')
heatmap2_data.head(n=5)
sns.heatmap(heatmap2_data, cmap="BuGn")
plt.show()

df2 = df[['Time','Distance', 'Direction','DNA Conc.']]
heatmap2_data = pd.pivot_table(df2,values='DNA Conc.', index=['Time'], columns='Distance')
heatmap2_data.head(n=5)
sns.heatmap(heatmap2_data, cmap="BuGn")
plt.show()


df3 = df[['Time','Distance', 'Direction','DNA Conc.']]
heatmap3_data = pd.pivot_table(df3,values='DNA Conc.', index=['Distance','Time'], columns='Direction')
