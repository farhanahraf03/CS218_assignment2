**Testing in AWS Cloud**
- Step 1 = Introduction - Download and install Python, Docker and SAM
- Step 2 = Project Setup - Building and deploying with SAM CLI
- Step 3 = Local testing - Working with SAM Events and SAM API Gateway emulators
- Step 4 = Testing in Cloud - Invoking Lambda function and running integration tests
- Step 5 = Observability - Fetching SAM logs and using AWS X-ray to trace invocations of AWS Lambda
- Step 6 = Cleanup - Delete the Cloudformation template, thereby deleting all the resources that arre created by that template

**Key takeaways**
- Basics of cloudformation templates and how they can be used to setup and cross reference AWS infrastructure
- basics of unit testing using pytest framework
- Uses API gatewway and how it can be used to trigger AWS Lambda functions
- Using syntethic events to invoke a Lambda function
- Using SAM acclerate to reduce deployment latency and test code quickly in AWS cloud
- SAM logs can be used for observability to fetch logs that are generated when Lambda is invoked due to API Gateway
- X-ray is used for metric tracing when we want to see details of AWS Lambda and trace it
- Integration test can be used to confirm if permissions are correctly configured or not
- SAM has API gateway emulator that emulates the performance of an API gateway and runs locally

**Bugs found**
- mock_s3 is deprecated in the latest versions -> use mock_aws instead
- Pytest cache issues can be overriden by using the no caching command -> py.test -p no:cacheprovider

**Screenshots**

![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/f272ccaa-d9b7-4a2a-bf62-c487f08b1e9c)

Bug found
![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/33440da4-fc66-4d81-a5b2-9950928cbce5)

Bug resolution
![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/a5266721-da6e-47ab-b402-d99ece54aace)

Pytest unit test cases
![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/95ffe90d-6816-4a0f-979e-f5c97904a610)

Integration tests
![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/ce30815b-817b-4880-9014-0250b1634e34)

Cloudformation builds
![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/d775ebb2-e6a9-42ee-9801-f4a14a918b9c)

Cloudformation output from deployed stack
![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/6c67cb54-54f6-431c-a058-fe579959ca41)

Tail of SAM logs for obersvability
![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/d43f4762-981d-4a09-a516-970f454dff9a)

Invoking API gaetway endpoint
![image](https://github.com/farhanahraf03/CS218_assignment2/assets/42094234/ef3f3bca-74e9-43f3-9068-8bb9d079c2bc)


