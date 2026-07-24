# Dataset Schema

## india-postal-lgd-mapping.csv

| Column | Type | Description |
| --------- | ------ | ------------- |
| pincode | string | 6-digit postal code |
| state | string | State Name |
| district | string | District Name |
| blocks | array | Matching blocks |
| state_lgd | string | State LGD Code |
| district_lgd | string | District LGD Code |

---

## india-postal-by-pincode.json

Structure

```json
{
  "110001": {
    "state": "...",
    "stateLGD": "...",
    "districts": []
  }
}
```

---

## india-district-index.json

Structure

```json
{
  "states": {}
}
```
