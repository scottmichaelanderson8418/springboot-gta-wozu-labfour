deploy:
  provider: elasticbeanstalk
  skip_cleanup: true
  region: us-east-2
  app: springboot-gta-wozu-labfour
  env: Springbootgtawozulabfour-env
  zip_file: 'target/springboot-gta-wozu-labfour-0.0.1-SNAPSHOT.jar'
  bucket_name: elasticbeanstalk-us-east-2-693831461729
  bucket_path: springboot-gta-wozu-labfour
  on: 
    branch: main
  access_key_id: $AWS_ACCESS_KEY_ID
  secret_access_key: $AWS_SECRET_ACCESS_KEY