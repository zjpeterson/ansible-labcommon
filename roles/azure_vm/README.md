# azure_vm
Creates a VM in Azure. Assumes that a Resource Group for the VM already exists which should be provided using `azure_vm_rg`.

The role outputs connection information at the end. It also runs `add_host` if you want to follow on with further configuration.

