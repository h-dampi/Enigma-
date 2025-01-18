# Zeno
Welcome to Zeno AI - Your Ultimate AI Evaluation Platform!
Introduction
Zeno AI is an innovative, open-source framework designed for comprehensive AI model evaluation and data management. It provides a powerful combination of a Python API and an interactive user interface, enabling developers, researchers, and data scientists to explore, visualize, and analyze the performance of their AI models across diverse use cases12.
Key Features
Zeno AI offers a wide range of features to streamline the AI evaluation process:
Data Exploration: Visualize various data types, including images, text, audio, and sensor data3.
Error Discovery: Automatically surface systematic failures in your models using advanced techniques like slice finder3.
Interactive Visualizations: Create beautiful, customizable charts to compare model performance across different slices and models3.
Report Authoring: Generate comprehensive reports with interactive visualizations and markdown text3.
Customizable Views: Support for multiple AI tasks, from chatbot conversations to object detection and audio transcription7.
Collaborative Tools: Author and publish reports collaboratively3.
Getting Started
To begin using Zeno AI, follow these steps:
Install the Zeno client:
bash
pip install zeno-client
Initialize the client and create a project:
python
from zeno_client import ZenoClient, ZenoMetric

client = ZenoClient(YOUR_API_KEY)
project = client.create_project(name="Writing Assistant", view="text-classification")
Upload your dataset and system outputs:
python
project.upload_dataset(df, id_column="id", data_column='text', label_column="label")
project.upload_system(system_df, name="GPT-4", id_column="id", output_column="output")
Community & Support
Join our growing community of AI practitioners using Zeno AI! Share your projects, ask questions, and collaborate with fellow enthusiasts to expand the possibilities of AI evaluation.
For support and assistance, visit our GitHub repository or reach out to our team through the official Zeno AI website.
License
Zeno AI is open-source software. For detailed licensing information, please refer to the LICENSE file in the repository.
Get started with Zeno AI today and unlock powerful insights into your AI models' performance!
