**Testing in AWS Cloud
**
- Step 1 = Introduction - Download and install Python, Docker and SAM
- Step 2 = Project Setup - Building and deploying with SAM CLI
- Step 3 = Local testing - Working with SAM Events and SAM API Gateway emulators
- Step 4 = Testing in Cloud - Invoking Lambda function and running integration tests
- Step 5 = Observability - Fetching SAM logs and using AWS X-ray to trace invocations of AWS Lambda
- Step 6 = Cleanup - Delete the Cloudformation template, thereby deleting all the resources that arre created by that template

**Key takeaways
**
- Basics of cloudformation templates and how they can be used to setup and cross reference AWS infrastructure
- basics of unit testing using pytest framework
- Uses API gatewway and how it can be used to trigger AWS Lambda functions
- Using syntethic events to invoke a Lambda function
- Using SAM acclerate to reduce deployment latency and test code quickly in AWS cloud
- SAM logs can be used for observability to fetch logs that are generated when Lambda is invoked due to API Gateway
- X-ray is used for metric tracing when we want to see details of AWS Lambda and trace it
- Integration test can be used to confirm if permissions are correctly configured or not
- SAM has API gateway emulator that emulates the performance of an API gateway and runs locally

**Bugs found
**
- mock_s3 is deprecated in the latest versions -> use mock_aws instead
- Pytest cache issues can be overriden by using the no caching command -> py.test -p no:cacheprovider

**Screenshots**
- Step 1 = Introduction - Download and install Python, Docker and SAM

