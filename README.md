# first
# command for build
packer build \
    -var 'aws_access_key=AKIAXOQ3XLO2NVDRX3W7' \
    -var 'aws_secret_key=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' \
    -var 'aws_region=us-east-1' \
    -var 'subnet_id=' \
    -var 'nonprod_account_id=813034945358'\
    -var 'ssh_username=ubuntu'
    ubuntu-ami.json
* second way
packer build -var-file=./vars.json ubuntu-ami.json
# may fail try oncemore

# trigger circleci
* curl -u 078489e257cd76aa7a874c4bc9c24b2b45d912bd -d build_parameters[CIRCLE_JOB]=build-base https://circleci.com/api/v1.1/project/github/majun2-spring2020/ami