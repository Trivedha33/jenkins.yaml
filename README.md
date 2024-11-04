stages:
  - build
  - test
  - deploy
 
variables:
  # Define any global variables here
 
before_script:
  # Commands to run before each job, like setting up dependencies
 
build_job:
  stage: build
  script:
    - echo "Building the project..."
    - # Add your build commands here
 
test_job:
  stage: test
  script:
    - echo "Running tests..."
    - # Add your test commands here
 
deploy_job:
  stage: deploy
  script:
    - echo "Deploying the project..."
    - # Add your deployment commands here
  only:
    - master
    # jenkins.yaml
