variable "resource_group_name" {
  type        = string
  description = "The name of the target Azure Resource Group"
  default     = "rg-devsecops-prod"
}

variable "location" {
  type        = string
  description = "The Azure region for the deployment"
  default     = "East US"
}

variable "vnet_cidr" {
  type        = list(string)
  description = "The core CIDR block for the Virtual Network"
  default     = ["10.0.0.0/16"]
}
