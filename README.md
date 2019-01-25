# aws-lambda-cloudformation
Deploy lambda with js file with cloudformation

### How to use 
```
aws cloudformation deploy \
  --template-file ./MyLambdaFunction.yaml \
  --stack-name MyLambdaFunction \
  --parameter-overrides \
    LambdaFunctionContents="$(<./MyLambdaFunction.js)" \
  --capabilities CAPABILITY_NAMED_IAM
```
