
# Customer Segmentation and Product Recommendation System

This project implements a customer segmentation and product recommendation system using machine learning techniques. The application is deployed using Docker and Ansible, and provides a Gradio interface for user interaction.

## Table of Contents
- Introduction
- Features
- Installation
- Usage
- Project Structure
- Contributing
- License

## Introduction
This project aims to segment customers based on their purchasing behavior and recommend products to them. It uses K-Means clustering for segmentation and Nearest Neighbors for product recommendations. The application is deployed in a Docker container and managed using Ansible.

## Features
- Customer segmentation using K-Means clustering.
- Product recommendations based on customer purchase history.
- Interactive Gradio interface for user input and output.
- Deployment using Docker and Ansible.

## Installation
### Prerequisites
- Docker
- Ansible

### Steps
1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/customer-segmentation-project.git
    cd customer-segmentation-project
    ```

2. **Set up the Docker container:**
    - Ensure Docker is installed and running.
    - Build and run the Docker container using Ansible:
      ```bash
      ansible-playbook -i hosts.ini deploy_gradio_app.yml --ask-become-pass
      ```

## Usage
1. **Access the Gradio interface:**
    - Open your web browser and go to `http://localhost:7860`.

2. **Interact with the application:**
    - Enter a Customer ID and the number of recommendations to get product recommendations based on purchasing behavior.

    Example IDs to test
    - 17850
    - 13047
    - 12583
    - 13748
    - 15100
    - 15291
    - 14688

## Project Structure
```
customer-segmentation-project/
├── data/
│   └── Online_Retail.xlsx
├── notebooks/
│   └──customer_segmentation.ipynb
├── src/
│   └── customer_segmentation.py
├── deploy_gradio_app.yml
├── dockerfile
├── hosts.ini
├── README.md
├── requirements.txt
```