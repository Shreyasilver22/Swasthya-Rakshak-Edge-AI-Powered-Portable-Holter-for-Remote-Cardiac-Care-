Project Name: Swasthya-Rakshak (Health Protector)

The Problem: Cardiovascular Diseases (CVDs) are the leading cause of mortality in India, yet quality cardiac monitoring is restricted to urban hospitals. Traditional Holter monitors are bulky, expensive, and require offline analysis by doctors, leading to fatal delays in diagnosis. In rural India ("Bharat"), patients often cannot access continuous monitoring until it is too late.

The Solution: Swasthya-Rakshak is a low-cost, IoT-enabled portable Holter monitor that democratizes cardiac care. Unlike passive recorders, our device uses an Intelligent Edge Computing architecture to detect arrhythmias (irregular heartbeats) in real-time.

Sensing: The AD8232 sensor captures high-fidelity ECG signals.

Edge Processing: A localized Edge AI Node performs noise filtration (DSP) and runs a lightweight ML model (XGBoost) to flag anomalies instantly without internet.

Cloud Analytics: Data is streamed to Google Cloud Platform (GCP) for deep-learning analysis, long-term trend tracking, and alerting doctors remotely.

Technical Architecture:

Hardware: Biomedical Sensor Node (AD8232) + Edge Computing Unit.

Cloud: Google Cloud Pub/Sub (Ingestion), Vertex AI (Anomaly Detection), Streamlit (Doctor's Dashboard).

Algorithms: Signal Processing (DSP) & Machine Learning (XGBoost) for PQRST wave classification.
