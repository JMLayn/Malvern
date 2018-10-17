# Malvern
Malven AAA workshop

These are all the commands that are executed in the InSpec workshop

```ssh azureuser@<your ip> (My-12-Char-Password)
  
touch firstname-lastname

ls -lt

sudo grep PermitRootLogin /etc/ssh/sshd_config

inspec --help

inspec init profile ~/profiles/ssh

tree ~/profiles/ssh

rm /home/azureuser/profiles/ssh/controls/example.rb

cp ~/.PermitRootLogin.rb ~/profiles/ssh/controls/PermitRootLogin.rb

sudo inspec exec profiles/ssh

inspec exec profiles/ssh -t ssh://azureuser@104.211.54.213 --password My-12-Char-Password --sudo

cat reporter.json

sudo inspec exec profiles/ssh --json-config reporter.json

cat .chef/cookbooks/ssh-remediation/recipes/default.rb

cat .chef/cookbooks/ssh-remediation/templates/sshd_config.erb -n

chef-run azureuser@localhost ssh-remediation::default --password My-12-Char-Password --config .chef-workstation/config.toml

sudo inspec exec profiles/ssh

sudo inspec exec profiles/ssh/ --json-config reporter.json```


