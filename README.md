# dac_IoT


## Configuration Management

### Prerequisites / assumptions
* SSH keys are used

  Best practice is to use puttygen to generate a secure key with a **passphrase** (long + strong cypher) and pageant to load the key and not have to always enter the passphrase. Populate the ~pi/.ssh/authorized_keys file with the public key generated above
* the user pi is allowed to run sudo without a password on the Raspberry PIs
* a control machine is used where ansible is installed (version >= 2.3.0.0)

### Invoking
`ansible-playbook -i inventory dataloggers.yml`
