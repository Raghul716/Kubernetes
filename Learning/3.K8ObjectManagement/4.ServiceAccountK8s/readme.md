In K8s, Service Account used by container process to Authenticate with K8s APIs.

If Pods needs to communicate with K8s APIs. User need to setup service account to control the access.

Service account can be created like any other Kubernetes Object using YAML file.

====================================
apiVersion: v1
kind: ServiceAccount
metadata:
name: my-serviceaccount
automountServiceAccountToken: false
====================================

# Role Binding Service Accounts

Service Account Access also manage by RBAC.

Bind Service Accounts with Cluster Role or ClusterRoleBinding to provide access to Cluster APIs.

====================================
apiVersion: rbac.authorization.k8s.io/v1
kind: RoleBinding
metadata:
 name: sa-pod-reader
 namespace: development
subjects:
- kind: ServiceAccount
 name: my-serviceaccount
 namespace: development
roleRef:
 kind: Role
 name: pod-reader
 apiGroup: rbac.authorization.k8s.io
====================================



