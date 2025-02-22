# End-to-End-Medical-Chatbot

![End-to-End Medical Chatbot](https://github.com/Supun-Dissanayaka/End-to-End-Medical-Chatbot-Using-Llama2/blob/main/Output/Chatbot.png?raw=true)

## Steps to run the project

```bash
conda create -n mchatbot python=3.8 -y
```

```bash
conda activate mchatbot
```

```bash
pip install -r requirements.txt
```


### Create a `.env` file in the root directory and add your Pinecone credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


### Download the quantize model from the link provided in model folder & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin

## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```


```bash
# run the following command
python store_index.py
```

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
- AWS
