# aws 계정변경
- export AWS_DEFAULT_PROFILE=$1
- 계정 변경확인 : aws s3 ls


# serverless + typescript + node.js
-> https://levelup.gitconnected.com/creating-a-simple-serverless-application-using-typescript-and-aws-part-1-be2188f5ff93    
-> https://chamch-dev.tistory.com/16      
-> https://gyuha.tistory.com/515


# node 버전 변경
-> https://jojoldu.tistory.com/569    
nodeenv 설치 // 17버전에서는 api 관련 특정에러 발생 // 16버전으로 사용할것 



# credential 따라 다르게 배포
-> serverless deploy --aws-profile $profilename

# 플러그인 
-> serverless-prune-plugin : 최근 버전남 남기도록


# serverless.yml config 
## provider
~~~
stage: ${opt:stage, 'dev'} -> -s 옵션을 받으면 사용하고, 그렇지 않으면 기본 dev 스테이지 사용
~~~
