

## 1- Init


#### 1.1- Init ENV
init environment variable
```sh
echo "set AWS_ACCESS_KEY_ID"
export AWS_ACCESS_KEY_ID="yourkeyid"
echo "set AWS_SECRET_ACCESS_KEY"
export AWS_SECRET_ACCESS_KEY="youraccesskey"
echo "set AWS_REGION"
export AWS_REGION="ap-northeast-1"
```


#### 1.2- Init `./project.json`

copy from

![image](https://user-images.githubusercontent.com/5538753/70849884-688ed780-1ebf-11ea-9ae0-6b22a5f26b52.png)


to `./project.json`
```json
{
    ...
    "role": "arn:aws:iam::293503197324:role/lambda"
}
```

## Deploy

Run
```
$ apex deploy bar foo
```

and you will see this in terminal
![image](https://user-images.githubusercontent.com/5538753/70849920-ca4f4180-1ebf-11ea-8adf-6683c1163a56.png)

and seeing the new functions on lambda
![image](https://user-images.githubusercontent.com/5538753/70849955-21551680-1ec0-11ea-90a1-4700e2b31f74.png)



