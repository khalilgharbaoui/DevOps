# DevOps

```
aws cloudformation create-stack \
  --template-body "$(cat vpc.json)" \
  --parameters "$(cat parameters.json)" \
  --stack-name "$(whoami)"
```

```
aws cloudformation update-stack \
  --template-body "$(cat vpc.json)" \
  --parameters "$(cat parameters.json)" \
  --stack-name "$(whoami)"
```

```
aws cloudformation delete-stack \
  --stack-name "$(whoami)"
  
```
