This is the deployment for the Beacon5G RAN digital twin
The deployment files are for two data centres dc1 and dc2 in the respective folders. The deployment scripts are kubernetes YAML files that support integration with federated consul service meshes.
The annotations required for injection of sidecars are :
      annotations:
        consul.hashicorp.com/connect-inject: 'true'

If license files are needed for the digital twin deployment (such as Matlab) then they should be available in the licenses-pv-claim Persistent volume. 

The purpose of the digital twin is to model the RAN elements in order to permit comparison of performance with the real ORAN system. This can help with selecting of optimal scheduling schemes and also detection and identification of the cause of differences between the models and the real system. 
