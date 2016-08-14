# corenlp-docker
corenlp-docker provides a dockerised version of the [Stanford CoreNLP Server](https://stanfordnlp.github.io/CoreNLP/corenlp-server.html).

## Simple usage

To pull the image and start the server, run:
```
docker run --rm -p 9000:9000 konradstrack/corenlp
curl --data 'A rather short sentence.' http://localhost:9000
```

For more complex examples of using the API, please refer to
[the official documentation](https://stanfordnlp.github.io/CoreNLP/corenlp-server.html) of CoreNLP Server.

## Building the image

```
docker build -t mycorenlp .
docker run --rm -p 9000:9000 mycorenlp
```
