# Demo GPT-OSS with Ollama

This page has simple steps to help you try [GPT-OSS](https://openai.com/index/introducing-gpt-oss/) with [Ollama](https://ollama.com/).

This page is intentionally as simple as possible to get our teammates up and running.

## Install

Install ollama.

If you want to use curl:

```sh
curl -fsSL https://ollama.com/install.sh | sh
```

If you want to use macOS and brew:

```sh
brew install ollama
```

## Serve

Start the server.

If you want to start ollama directly:


```sh
ollama serve
```

If you want to use macOS and brew to start the ollama server in the background:

```sh
brew services start ollama
```


## Pull

Pull a GPT-OSS model, which means your system will download the model.

```sh
ollama pull gpt-oss:20b
```

## Run

Run the model, which means the Ollama server will launch the model, and show you a prompt where you can type and interact with the model.


```sh
ollama run gpt-oss:20b
```

## Bonus

If you have a powerful system, such as a computer with lots of RAM and many GPU cores, then you may want to experiment with the larger model.

Pull:

```sh
ollama pull gpt-oss:120b
```

Run:

```sh
ollama run gpt-oss:120b
```

## Speed

On a MacBook M4 Max, the larger model works very well for personal chat interactions.

A simple request takes 2-4 seconds or so: "explain agile software development".

A longer request takes 10-20 seconds, and shows the chain of thought in progress: "explain agile software development (one paragraph introduction then bullet points) (between 220 and 250 words)".

## Thanks

Thanks for all the developers who are creating this open source software.

Constructive suggestions about this page are welcome: <joel@joelparkerhenderson.com>.
