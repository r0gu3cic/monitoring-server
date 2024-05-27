# Monitoring server

This is a automation project for creating a monitoring server image that could be reusable on a Cloud Provider such as DigitalOcean.  
Monitoring server will have installed Prometheus, Node Exporter, Alertmanager and Grafana service and will monitor itself (I know, I know, but this is a hobby project and I don't want to waste money on creating multiple servers).  
Once server is created and tested, image will be created and that image should be final product of this code. If we spawn server image created like this it should work out-of-the-box with minimal config.  
The idea is to provision server using Terraform, configure it using Ansible, create server image using Terraform and finally delete everything except image using Terraform.  
Furthermore I will implement GitHub Actions workflow for creating new image whenever there is a code change.  
