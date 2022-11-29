# emlov2_session09
lambda inference engine


Link to Backend deployed Lambda-
https://wpbivowat2.execute-api.ap-northeast-1.amazonaws.com/dev/inference

Sample Request Body-

```
{"body": "data:image/png;base64,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"
}
```

Model restnet18 was trained on CIFAR image set and stored as jit script

Code deployment done by leveraging serverless framework

```
curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -

sudo apt install nodejs
sudo npm i -g serverless

serverless deploy

```



