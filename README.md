# sit323_737-2023-t1-prac7c

# Docker container running on the kubenetes cluster

- Image Name: bpritch/web-node-app

1. Create token for the cluster 'kubectl -n kubernetes-dashboard create token admin-user'.
2. Run 'kubectl proxy' to start the proxy.
3. Login to the dashboard with the following link:
   http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/
4. Enter the token created in step 1.
5. Port forwarding - 'kubectl port-forward service/web-node-app 8001:8001'
6. Access the calculator app at http://localhost:8001
7. Log in with either user1/user2 & password1/password2
