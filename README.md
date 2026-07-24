# 🇮🇳 India Postal Pincode Dataset

🇮🇳 Comprehensive India Postal Pincode dataset containing 20,144 postal records with State, District, Block, and LGD code mappings, available in CSV and JSON formats.

## Features

- 20,144 unique postal records
- State LGD codes
- District LGD codes
- Block mappings
- CSV and JSON formats
- Fast pincode lookup
- District index for GIS applications

## Folder Structure

```text
csv/
    india-postal-lgd-mapping.csv

json/
    india-postal-by-pincode.json
    india-district-index.json

docs/
    schema.md
```

## Dataset

### CSV

| Column | Description |
| --------- | ------------- |
| pincode | 6-digit India Postal Code |
| state | State Name |
| district | District Name |
| blocks | Associated Blocks |
| state_lgd | State LGD Code |
| district_lgd | District LGD Code |

---

### JSON

#### india-postal-by-pincode.json

Fast lookup by pincode.

Example

```json
{
  "110001": {
    "state": "DELHI",
    "stateLGD": "07",
    "districts": [
      {
        "district": "NEW DELHI",
        "districtLGD": "094",
        "blocks": [
          "NEW DELHI"
        ]
      }
    ]
  }
}
```

---

#### india-district-index.json

Lookup districts by state and obtain LGD metadata.

Example

```json
{
  "states": {
    "ANDHRA PRADESH": {
      "ANAKAPALLI": {
        "districtLGD": "685",
        "jsonFile": "ANDHRA PRADESH.json"
      }
    }
  }
}
```

## Typical Use Cases

- Address validation
- GIS applications
- Government projects
- Education platforms
- Analytics dashboards
- Pincode autocomplete
- Location mapping
- State & District lookups

## Notes

- LGD refers to the Local Government Directory maintained by the Government of India.
- Block values are derived from postal data and administrative mappings.

## License

MIT License
