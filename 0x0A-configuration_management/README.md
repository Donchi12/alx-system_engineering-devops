# 0x0A. Configuration management

## Resource



```sh
# installing puppet and puppet-lint
wget https://apt.puppet.com/puppet7-release-focal.deb && \
    dpkg -i puppet7-release-focal.deb && \
    apt-get update && \
    apt-get install puppet-agent puppet-lint -y

# confirming installation
puppet -V
puppet-lint -v

# If you get an error saying puppet command not found, source the path
source /etc/profile.d/puppet-agent.sh

