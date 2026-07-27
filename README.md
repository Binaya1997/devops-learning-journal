# DevOps Learning Journal

## Day 1: Local AWS with Floci

### What I Did
- Installed Floci (local AWS emulator)
- Configured AWS CLI with fake credentials pointing to localhost:4566
- Created S3 bucket: `my-first-floci-bucket`
- Uploaded and downloaded a test file via CLI

### Commands Used
```bash
floci start
aws s3 mb s3://my-first-floci-bucket --endpoint-url http://localhost:4566
aws s3 cp hello.txt s3://my-first-floci-bucket/ --endpoint-url http://localhost:4566
aws s3 ls s3://my-first-floci-bucket/ --endpoint-url http://localhost:4566
