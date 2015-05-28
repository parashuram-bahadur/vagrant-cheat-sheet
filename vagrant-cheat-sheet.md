Typing `vagrant` from the command line will display a list of all available commands.

# Common Vagrant Commands
- `vagrant up`            -- starts vagrant environment (also provisions only on the FIRST vagrant up)
- `vagrant status`        -- outputs status of the vagrant machine
- `vagrant global-status` -- outputs status of all vagrant machines
- `vagrant halt`          -- stops the vagrant machine
- `vagrant reload`        -- restarts vagrant machine, loads new Vagrantfile configuration
- `vagrant provision`     -- forces reprovisioning of the vagrant machine
- `vagrant ssh`           -- connects to machine via SSH
- `vagrant destroy`       -- stops and deletes all traces of the vagrant machine

# Tips
- `vagrant -v`                  -- Get the vagrant version
- `vagrant suspend`             -- Suspends a virtual machine (remembers state)
- `vagrant resume`              -- Resume a suspended machine (vagrant up works just fine for this as well)
- `vagrant reload --provision`  -- Restart the virtual machine and force provisioning
- `vagrant push`                -- Yes, vagrant can be configured to [deploy code](http://docs.vagrantup.com/v2/push/index.html)!
- `vagrant up --provision | tee provision.log`  -- Runs `vagrant up`, forces provisioning and logs all output to a file