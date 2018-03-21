# HEAT

In this repo i will share some HOT examples 


### HOT_server_with_complete_resources.yaml

In this HOT file i create a server with a complete non-existing resources. so every resource will be related to this stack.

- server
- internal & external networks with thier subnet
- router with a floting ip attached to the server
- keypair
- security group

the resources variables can be configured using the [ENV_server_with_complete_resources.yaml](https://github.com/ibragh/OpenStack/tree/master/heat#env_server_with_complete_resourcesyaml)

##### How to run:

--wait : Wait for creating to reach the CREATE_COMPLETE status. it will show a simple log to monitor what is going while creating the stack


```

$ openstack stack create --template HOT_server_with_complete_resources.yaml \
	--environment ENV_server_with_complete_resources.yaml \
	--wait mystack

```


### ENV_server_with_complete_resources.yaml

Environment parameters related to [HOT_server_with_complete_resources.yaml](https://github.com/ibragh/OpenStack/tree/master/heat#hot_server_with_complete_resourcesyaml)
