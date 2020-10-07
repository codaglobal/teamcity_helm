# Helm Chart for TeamCity
This is a simple chart that stands up a single Server and Agent.
By default, it uses EmptyDir for Volumes and Ingress is disabled.

## Key Values
- agentReplicaCount: The number of Agents that will be created (default: 1)
- pvc.data: A PVC name for the Data directory on the Server (default: "").
- pvc.logs: A PVC name for the Logs directory on the Server (default: "").
- pvc.config: A PVC name for the configuration on the Agent (default: "").
- ingress.enabled: Set to true to enable Ingress
- ingress.hosts: Array of Host entries for Ingress

# TODO
Add this as a packaged Chart with install instructions