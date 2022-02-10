---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "jwks_from_pem Data Source - terraform-provider-jwks"
subcategory: ""
description: |-
  Calculates a JSON Web Key Set from a given public or private key.
---

# jwks_from_pem (Data Source)

Calculates a JSON Web Key Set from a given public or private key.

## Example Usage

```terraform
data "jwks_from_pem" "test" {
  pem = <<EOF
-----BEGIN PUBLIC KEY-----
MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAgUElV5mwqkloIrM8ZNZ7
2gSCcnSJt7+/Usa5G+D15YQUAdf9c1zEekTfHgDP+04nw/uFNFaE5v1RbHaPxhZY
Vg5ZErNCa/hzn+x10xzcepeS3KPVXcxae4MR0BEegvqZqJzN9loXsNL/c3H/B+2G
le3hTxjlWFb3F5qLgR+4Mf4ruhER1v6eHQa/nchi03MBpT4UeJ7MrL92hTJYLdpS
yCqmr8yjxkKJDVC2uRrr+sTSxfh7r6v24u/vp/QTmBIAlNPgadVAZw17iNNb7vjV
7Gwl/5gHXonCUKURaV++dBNLrHIZpqcAM8wHRph8mD1EfL9hsz77pHewxolBATV+
7QIDAQAB
-----END PUBLIC KEY-----
EOF
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **pem** (String) Required pem encoded public or private key.

### Optional

- **id** (String) The ID of this resource.

### Read-Only

- **jwks** (String) The calculated JSON Web Key Sets.

