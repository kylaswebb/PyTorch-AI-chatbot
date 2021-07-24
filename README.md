<h1 align="center">:robot: PyTorch AI-Chatbot for E-commerce Site :computer:</h1>

In conversations, Context is king. This is a chatbot framework with a conversational model for an Ecommerce Website. The chatbot handles simple questions about hours of operation, reservation options, products in stock and so on. The chatbot also handles contextual responses such as inquiries about same-day deliveries and shipping. 

## :electric_plug: What to Expect
- Training of the chatbot

![Training of the chatbot](https://user-images.githubusercontent.com/62080362/126873091-fb884e3d-ef65-4f50-a8ee-cccf83449ca4.png)

- Chatbot running in the CLI

![Chatbot running in CLI](https://user-images.githubusercontent.com/62080362/126873127-f694e106-a22c-45fe-8d28-c07a254bb8bf.png)

## :syringe:Installation

### :earth_africa:Create an environment
- Whatever you prefer (e.g. `conda` or `venv`)
```console
mkdir myproject
$ cd myproject
$ python3 -m venv venv
```

### :hotsprings:Activate it
- For Mac / Linux users:
```console
. venv/bin/activate
```
- For Windows Users: 
Use `conda base activate` or the code below:
```console
venv\Scripts\activate
```
### :thermometer:Install PyTorch and it's dependencies

- For Installation of PyTorch see [official website](https://pytorch.org/).
- You also need `nltk`:
 ```console
pip install nltk
 ```
- If you get an error during the first run, you also need to install `nltk.tokenize.punkt`:
- Run this once in your terminal:
 ```console
$ python
>>> import nltk
>>> nltk.download('punkt')
```

## :high_brightness:Usage
- Run
```console
python train.py
```
- This will dump data into the `data.pth` file. And then run
```console
python chat.py
```

## :gear:Customize
- Have a look at [intents.json](intents.json). 
- You can customize it according to your own use case. Define a new `tag`, possible `patterns`, and possible `responses` for the chat bot. You have to re-run the training whenever this file is modified.
```console
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": [
        "Hi",
        "Hey",
        "How are you",
        "Is anyone there?",
        "Hello",
        "Good day"
      ],
      "responses": [
        "Hey :-)",
        "Hello, thanks for visiting",
        "Hi there, what can I do for you?",
        "Hi there, how can I help?"
      ]
    },
    ...
  ]
}
```

## :v:Contributing

- You wanna contribute? Wow amazing. That's great to hear.
- After cloning & setting up the local project you can push the changes to your github fork and make a pull request.

### :chart_with_upwards_trend:Pushing the changes

```bash
git add .
git commit -m "feat: added new stuff"
git push YOUR_REPO_URL BRANCH_NAME
```

---

<h3 align="center"> This code was built with :heart: and alot of Coffee:coffee:</h3>
