# Asset Classes (SSOT)

This folder is the **single source of truth** for:
- master templates per asset class
- required fields (machine-readable)
- provider inquiry question blocks (DOC-10-00-A)

## Structure

```
asset-classes/
  <class-slug>/
    master-intake.md          # DOC-10-00 master (per class)
    master-provider.md        # DOC-10-00-A master (per class)
    required-fields.json      # required fields + units + mapping targets
    questions-provider.md     # derived questions for missing required fields
```

## Notes
- GitHub is SSOT; OneDrive is only for file exchange.
- When a new class is introduced, create the folder first before processing assets.
