# dac_IoT

## Basic git workflow
Currently all changes are pushed to the master branch by commiters and the typical workflow looks something like:
* git clone git@github.com:ppaul72/dac_IoT.git



## Configuration Management

### Prerequisites / assumptions
* SSH keys are used

  Best practice is to use ssh keys (puttygen on windows) with a **passphrase** (long + strong cypher) and an ssh agent (pageant on windows) to load the key and not have to always enter the passphrase. Populate the ~pi/.ssh/authorized_keys file with the public key generated above
* the user pi is allowed to run sudo without a password on the Raspberry PIs
* a control machine is used where ansible is installed (version 2.3.0.0 at the time of writing)

### Invoking
`ansible-playbook -i inventory dataloggers.yml`
