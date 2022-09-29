# JsonPredicateBuilder
## JSON Data for match

Json example for Build Predicate

```c#
{
  "condition": "and",
  "rules": [
    {
      "condition": "or",
      "rules": [
        {
          "field": "LastName",
          "operation": "IsEqualTo",
          "type": "ShortText",
          "primitive_value": "Poxosyan",
          "value_object": {}
        },
        {
          "field": "LastName",
          "operation": "IsEqualTo",
          "type": "ShortText",
          "primitive_value": "Hayrapetyan",
          "value_object": {}
        }

      ]
    },
    {
      "field": "Phone",
      "operation": "IsEqualTo",
      "type": "ShortText",
      "primitive_value": "5555555555",
      "value_object": {}
    },

    {
      "field": "FirstName",
      "operation": "Contains",
      "type": "ShortText",
      "primitive_value": "ik",
      "value_object": {}
    },

    {
      "field": "FirstName",
      "operation": "EndsWith",
      "type": "ShortText",
      "primitive_value": "ik",
      "value_object": {}
    },
    {
      "field": "FirstName",
      "operation": "StartsWith",
      "type": "ShortText",
      "primitive_value": "P",
      "value_object": {}
    },
    {
      "condition": "or",
      "rules": [
        {
          "field": "Age",
          "operation": "IsGreaterThen",
          "type": "Number",
          "primitive_value": 15,
          "value_object": {}
        },
        {
          "field": "Segments",
          "operation": "IsEqualTo",
          "type": "ShortText",
          "primitive_value": "sevaher",
          "value_object": {}
        },
        {
          "field": "CustomFields",
          "operation": "IsEqualTo",
          "type": "Object",
          "primitive_value": "",
          "value_object": {
            "FieldName": "A",
            "DefaultValue": {
              "value": "shortCustm"
            },
            "FieldType": "shortText"
          }
        },
        {
          "field": "CustomFields",
          "operation": "IsEqualTo",
          "type": "Object",
          "primitive_value": "",
          "value_object": {
            "FieldName": "B",
            "DefaultValue": {
              "value": "{\"IsMulty\":false,\"Values\":[\"A\",\"B\",\"C\",\"D\"],\"SelectedItems\":[\"B\"]}}"
            },
            "FieldType": "select"
          }
        }
      ]
    },
    {
      "field": "Addresses",
      "operation": "IsEqualTo",
      "type": "Object",
      "primitive_value": "",
      "value_object": {
        "Country": "Armenia",
        "City": "Yerevan",
        "State": "Arabkir",
        "Zip": "45678",
        "AddressLine1": "Chraenc",
        "AddressLine2": "Ulneci"
      }
    }
  ]
}
```
