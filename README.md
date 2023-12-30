# Medical-Chatbot-using-Llama2

## Steps to run the project

1. Clone the repository
```bash
git clone https://github.com/tejas05in/Medical-Chatbot-using-Llama2.git
```

2. create conda environment
```bash
conda create -p env python=3.8 -y
```
3. Activate conda environment
```bash
conda activate env/
```
4. Install requirements
```bash
pip install -r requirements.txt
```

5. Create a `.env` file in the root directory and add your Pinecone credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


6. Download the quantize model from the link provided in model folder & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin


## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

7. Storing the vector index
```bash
# run the following command
python store_index.py
```

8. Run the flask app
```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up localhost:
```


### Techstack Used:

- Python
- LangChain
- Flask
- Meta Llama2
- Pinecone
