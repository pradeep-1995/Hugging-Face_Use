# **Question Answering and Text Generation Chatbot**

This repository hosts a Question Answering and Text Generation chatbot built using Hugging Face's Transformers and FastAPI. The project fine-tunes a BERT-based model for question answering and uses a GPT-based model for text generation. The API enables seamless integration with front-end applications for building interactive AI solutions.

---

## **Features**
1. **Question Answering**: Fine-tuned BERT model on the SQuAD dataset to provide accurate answers based on context.
2. **Text Generation**: GPT-based pipeline to generate contextually relevant text, such as motivational quotes.
3. **REST API**: Built with FastAPI for high-performance asynchronous endpoints.
4. **CORS Support**: Integrated middleware for cross-origin resource sharing.

---

## **Installation**

### **Prerequisites**
Ensure you have the following installed:
- Python 3.8 or later
- pip (Python package manager)

### **Steps**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/question-answering-chatbot.git
   cd question-answering-chatbot
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   uvicorn main:app --reload
   ```
4. Access the API documentation at `http://127.0.0.1:8000/docs`.

---

## **Endpoints**

### **1. Question Answering**
- **Path**: `/question-answer`
- **Method**: POST
- **Request Body**:
  ```json
  {
    "question": "What is the educational background of Pradeep?"
  }
  ```
- **Response**:
  ```json
  {
    "answer": "Pradeep earned his B.Tech in Electrical Engineering from BPUT and a Master's in Automation and Process Control from CTTC."
  }
  ```

### **2. Generate Quotes**
- **Path**: `/generate-quote`
- **Method**: GET
- **Response**:
  ```json
  {
    "quote": "The purpose of life is to find your purpose and give it your all."
  }
  ```

---

## **Documentation**

### **Directory Structure**
```
├── main.py                # FastAPI application
├── requirements.txt       # Required Python packages
├── README.md              # Project documentation
└── models/                # Pre-trained models (optional for manual download)
```

### **Technologies Used**
- **Models**: Hugging Face Transformers (`bert-base-cased`, `gpt-based`)
- **Framework**: FastAPI
- **Tokenizer**: Hugging Face Tokenizers
- **Serving**: Uvicorn

---

## **How to Fine-tune the Model**
1. Use the provided BERT-based `AutoModelForQuestionAnswering` to preprocess the dataset (e.g., SQuAD).
2. Define tokenization strategies and prepare the datasets for training and evaluation.
3. Fine-tune the model using TensorFlow or PyTorch with mixed precision for optimal performance.
4. Save the fine-tuned model and integrate it with the FastAPI app.

---

## **Contributing**
1. Fork the repository.
2. Create a new branch for your feature/bug fix.
3. Submit a pull request with detailed changes.

---

## **License**
This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## **Contact**
For queries or suggestions, feel free to contact:
- **Pradeep Parida**: [pradeepparida919@gmail.com](mailto:pradeepparida919@gmail.com) 
## My Portfolio
- Welcome to my project repository! Check out my [Portfolio Website](https://pradeep-1995.github.io/Protfolio.github.io/) to see my complete work and experience.
---

### **Future Enhancements**
- Extend support for multilingual question answering.
- Improve model inference speed using ONNX.
- Add more text generation styles and themes. 

