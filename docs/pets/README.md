# pets

### Available Operations

* [createPets](#createpets) - Create a pet
* [listPets](#listpets) - List all pets
* [showPetById](#showpetbyid) - Info for a specific pet

## createPets

Create a pet

### Example Usage

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

## listPets

List all pets

### Example Usage

```typescript
import { SDK } from "test-petstore";
import { ListPetsResponse } from "test-petstore/dist/sdk/models/operations";

const sdk = new SDK();

sdk.pets.listPets({
  limit: 548814,
}).then((res: ListPetsResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

## showPetById

Info for a specific pet

### Example Usage

```typescript
import { SDK } from "test-petstore";
import { ShowPetByIdResponse } from "test-petstore/dist/sdk/models/operations";

const sdk = new SDK();

sdk.pets.showPetById({
  petId: "provident",
}).then((res: ShowPetByIdResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```
