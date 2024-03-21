Testing in AWS Cloud

- Create AWS Lambda and AWS API gateway using Cloudformation templates
- Perform Unit tests using Pytest framework

Bugs found
- mock_s3 is deprecated in the latest versions -> use mock_aws instead
- Pytest cache issues can be overriden by using the no caching command -> py.test -p no:cacheprovider

