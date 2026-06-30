# 🤖 AI Freelancer Assistant - Day 1

> A Streamlit-powered dashboard to help AI Freelancers manage proposals, track productivity, and monitor AI credits in one place.

---

## 📌 Project Status: Day 1 - MVP Dashboard

**Goal:** Build and deploy a functional Streamlit dashboard on Google Colab with public access.

### ✅ Features Implemented

| Feature | Description | Status |
| --- | --- | ---
| **Dashboard UI** | Clean, responsive layout using `st.set_page_config` and `st.columns` | Complete |
| **Key Metrics** | Displays core KPIs: Proposals, Cover Letters, AI Credits | Complete |
| **Recent Activity** | Text-based summary of proposals generated per day | Complete |
| **Public Deployment** | App exposed via `localtunnel` for client/instructor review | Complete |

### 🛠️ Tech Stack

- **Framework**: Streamlit v1.40+
- **Language**: Python 3.10+
- **Libraries**: Pandas, Plotly [Prepared for Day 2]
- **Environment**: Google Colab
- **Deployment**: LocalTunnel

### 🚀 How to Run Locally

```bash
pip install streamlit pandas plotly
streamlit run app.py
### 🌐 How to Run on Google Colab

1.  Run all cells in sequence.
2.  Execute the LocalTunnel cell.
3.  Open the generated `https://xxxx.loca.lt` URL in an Incognito window.
4.  Enter the displayed IP address to access the app.

### ⚠️ Known Limitation & Mitigation

*Issue*: `st.metric()` and `st.plotly_chart()` components fail to load via LocalTunnel due to JS module fetching errors on Colab. 

*Mitigation for Day 1*: Used `st.write()` for KPIs to ensure 100% app stability and successful submission. 

*Next Steps for Day 2*: Migrate to Streamlit Community Cloud for full support of `st.metric`, `st.plotly_chart`, and `streamlit-authenticator` for Login/Register functionality.

### 👤 Author

*Warda Ejaz*  
AI Freelancer Project | Day 1 Submission
