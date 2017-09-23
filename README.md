### Network Google Cloud Platform 

##### Example (minimum)

```hcl
module "network" {
  source = "github.com/tasdikrahman/tf-module-gcp-network"
  name   = "${var.name}"
}
```

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| auto_create_subnetworks | Auto-creation of the associated subnet | string | `false` | no |
| name | Network name to create on GCP | string | - | yes |

## Outputs

| Name | Description |
|------|-------------|
| gateway_ipv4 | The IPv4 address of the gateway |
| name | The unique name of the network |
| self_link | The URL of the created resource |

### LICENSE

MIT License
