# Medical-Chatbot-using-Llama2

## Steps to run the project

1. create conda environment
```bash
conda create -p env python=3.8 -y
```
2. Activate conda environment
```bash
conda activate env/
```
3. Install requirements
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the root directory and add your Pinecone credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


5. Download the quantize model from the link provided in model folder & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin


## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

6. Storing the vector index
```bash
# run the following command
python store_index.py
```

7. Run the flask app
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

