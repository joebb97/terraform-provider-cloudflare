---
page_title: "cloudflare_d1_database Resource - Cloudflare"
subcategory: ""
description: |-
  The D1 Database https://developers.cloudflare.com/d1/ resource allows you to manage Cloudflare D1 databases.
---

# cloudflare_d1_database (Resource)

The [D1 Database](https://developers.cloudflare.com/d1/) resource allows you to manage Cloudflare D1 databases.

!> When a D1 Database is replaced all the data is lost. Please ensure you have a backup of your data before replacing a D1 Database.


## Example Usage

```terraform
resource "cloudflare_d1_database" "example" {
  account_id = "f037e56e89293a057740de681ac9abbe"
  name       = "terraform-database"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `account_id` (String) The account identifier to target for the resource.
- `name` (String) The name of the D1 Database.

### Read-Only

- `id` (String) The identifier of this resource.
- `version` (String) The backend version of the database.

## Import


Import is supported using the following syntax:

```shell
$ terraform import cloudflare_d1_database.example <account id>/<database id>
```
