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