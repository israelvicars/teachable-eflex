# Teachable eFlex 

## About 
Styled and edited version of the Teachable Machine project for an internal demonstration of machine learning features integrated into the eFlex product suite.

![Animated gif demo](/teachable-eflex-demo.gif)

## Teachable Machine
[Teachable Machine](https://github.com/googlecreativelab/teachable-machine) is an experiment for exploring machine learning built using the [deeplearn.js](https://github.com/PAIR-code/deeplearnjs) library. Try it at [g.co/teachablemachine](https://g.co/teachablemachine). 

## Development

#### Install dependencies and build project 
```
yarn
yarn build
```

#### To start local http server
```
yarn run watch
```

#### To run https locally:
https is required to get camera permissions to work when not working with `localhost`

1. Generate Keys
```
openssl genrsa -out server.key 2048
openssl req -new -x509 -sha256 -key server.key -out server.cer -days 365 -subj /CN=YOUR_IP
```
2. Use `yarn run watch-https`
3. Go to `https://YOUR_IP:3000`, then accept the insecure privacy notice, and proceed.

## Credit
Teachable Machine project was made by [Støj](http://stoj.io/), [Use All Five](https://useallfive.com/) and Creative Lab and [PAIR](https://ai.google/pair/) teams at Google.
