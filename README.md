# test-petstore

<!-- Start SDK Installation -->
## SDK Installation

### NPM

```bash
npm add test-petstore
```

### Yarn

```bash
yarn add test-petstore
```
<!-- End SDK Installation -->

## SDK Example Usage
<!-- Start SDK Example Usage -->
```typescript
import { SDK } from "test-petstore";
import { CreatePetsResponse } from "test-petstore/dist/sdk/models/operations";

const sdk = new SDK();

sdk.pets.createPets().then((res: CreatePetsResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```
<!-- End SDK Example Usage -->

<!-- Start SDK Available Operations -->
## Available Resources and Operations


### [pets](docs/pets/README.md)

* [createPets](docs/pets/README.md#createpets) - Create a pet
* [listPets](docs/pets/README.md#listpets) - List all pets
* [showPetById](docs/pets/README.md#showpetbyid) - Info for a specific pet
<!-- End SDK Available Operations -->

### Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

### Contributions

While we value open-source contributions to this SDK, this library is generated programmatically.
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release !

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)

