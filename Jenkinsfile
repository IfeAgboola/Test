stages{
      stage('deploy to S3'){
          steps{
              sh 'aws s3 cp public/index.html s3://jenkinsbife'
              sh 'aws s3api put-object-acl --bucket jenkinsbife --key index.html --acl public-read'
              sh 'aws s3 cp public/error.html s3://jenkinsbife'
              
          }
      }
  }
