Vagrant Scripts
=========

Scripts I use with vagrant to make life easier


#V

Used to easily access vagrants from anywhere on a system.

###Usage
Global status of all registered vagrant machines:
```bash
v 
```

To run a vagrant command against a target machine:

```bash
v [COMMAND] [NAME]
```

###Installation

Copy v script to user bin directory:
```bash 
cp vagrant_anywhere/bin/v ~/bin/
```

Copy v autocomplete to bash_completion.d:
```bash
cp vagrant_anywhere/bash_completion/v ~/.bash_completion.d/v
```

Add the bash completion to .bash_profile:
```bash
. ~/.bash_completion.d/v
```

To name a VagrantBox add the config.vm.define to the VagrantFile:

```ruby
Vagrant.configure("2") do |config|
  ...
  
  config.vm.define "VAGRANT NAME HERE" do |foohost|
  end
  
  ...
```
