# Monitoring server

This is an automation project for creating a monitoring server image that could be reusable on a Cloud Provider such as DigitalOcean.  
The monitoring server will have installed Prometheus, Node Exporter, Alertmanager, and Grafana service. It will monitor itself (I know, I know, but this is a hobby project and I don't want to waste money on creating multiple servers).  
Once the server is created and tested, an image will be created and that image should be the final product of this code. If we spawn a server image created like this it should work out-of-the-box with minimal config.  
The idea is to provision the server using Terraform, configure it using Ansible, create a server image using Terraform, and finally delete everything except the image using Terraform.  
Additionally, I will implement a GitHub Actions workflow for creating new images whenever there is a code change.  
