stages{
      stage('deploy to S3'){
          steps{
              sh 'aws s3 cp public/index.html s3://<my-s3-jenkins-bucket>'
              sh 'aws s3api put-object-acl --bucket <my-s3-jenkins-bucket> --key index.html --acl public-read'
              sh 'aws s3 cp public/error.html s3://<my-s3-jenkins-bucket>'
              sh 'aws s3api put-object-acl --bucket <my-s3-jenkins-bucket> --key error.html --acl public-read'
          }
      }
  }
