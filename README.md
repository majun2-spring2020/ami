# first
# command for build
packer build \
    -var 'aws_access_key=AKIAXOQ3XLO2NVDRX3W7' \
    -var 'aws_secret_key=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' \
    -var 'aws_region=us-east-1' \
    -var 'subnet_id=' \
    ubuntu-ami.json