# Implementation of a Contextual Chatbot in Pytorch
This repository is all about building chatbot in Python programming language and by using Pytorch.
- This is just a simple implementation that includes simple & general intents like `greetings` & `Goodbye` & `Thanks` & ... .
- The implementation is straightforward with a Feed Forward Neural network with 2 hidden layers.
- The `intent.json` can be customized to fit for any other usecases with possible patterns and responses.



## Usage
Run
```console
python train.py
```
This will dump `data.pth` file. And then run
```console
python chat.py
```

## Customize
Have a look at [intents.json](intents.json). You can customize it according to your own use case. Just define a new `tag`, possible `patterns`, and possible `responses` for the chat bot. You have to re-run the training whenever this file is modified.
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

## Reference
[link](https://www.youtube.com/watch?v=RpWeNzfSUHw&list=PLqnslRFeH2UrFW4AUgn-eY37qOAWQpJyg)
