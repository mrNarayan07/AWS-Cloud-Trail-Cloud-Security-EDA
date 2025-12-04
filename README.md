# AWS CloudTrail Security EDA – Flaws.Cloud Dataset

This project performs **Exploratory Data Analysis (EDA)** on public **AWS CloudTrail logs** from the `flaws.cloud` environment to uncover security-relevant patterns such as suspicious IPs, high-risk API calls, and anomalous activity over time.

The goal is to help security analysts and students understand how to:
- Explore **CloudTrail logs**
- Visualize **attacks vs normal activity**
- Derive **security insights** from real-world data

---

## 📦 Dataset

- **Name:** AWS Cloudtrails Dataset from flaws.cloud  
- **Source (Kaggle):**  
  https://www.kaggle.com/datasets/nobukim/aws-cloudtrails-dataset-from-flaws-cloud  
- **Original logs & description:** Public CloudTrail logs from the `flaws.cloud` training environment, mostly containing **attacks against a real AWS account**, spanning ~3.5 years (2017–2020). :contentReference[oaicite:0]{index=0}  

The dataset contains anonymized CloudTrail events, including (but not limited to):

- `eventTime`
- `eventName`
- `eventSource`
- `awsRegion`
- `sourceIPAddress`
- `userAgent`
- `userIdentity.*`
- `errorCode`, `errorMessage`
- Custom derived columns (e.g., `status`) created during EDA

---

## 🧰 Tech Stack

- **Language:** Python (>= 3.9)
- **Core Libraries:**
  - `pandas` – data loading & wrangling  
  - `numpy` – numeric utilities  
  - `matplotlib`, `seaborn` – visualizations  
  - `jupyter` / `ipykernel` – notebooks (optional)

Install the basics:

```bash
pip install pandas numpy matplotlib seaborn jupyter

