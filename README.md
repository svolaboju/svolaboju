- 👋 Hi, I’m @svolaboju
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
svolaboju/svolaboju is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->import streamlit as st
import pandas as pd
import numpy as np
import plotly.figure_factory as ff
import matplotlib.pyplot as plt
st.title(‘breach_report’)
@st.cache
def load_data(nrows):
    data = pd.read_csv('breach_report.csv', nrows=nrows)
    return data
    data_load_state = st.text('Loading data...')

