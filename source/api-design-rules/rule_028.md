### ID 28

| Title    | __28 - Extensible enumerations__ |
| :----    | :---------- |
| Strategy | Use x-extensible-enum for open ended lists of values. |

<details><summary>

Open section for explanation, rationale and exception conditions 

</summary>

#### Explanation

An extensible enum is defined using the `x-extensible-enum`, like in the following example:

```yaml
energyType:
  type: string
  x-extensible-enum:
    - ELEK
    - GAS
```

#### Rationale

Whereas [enumerations](rule_021) are used for lists that have a well-defined scope and are not intended for extension (except as a breaking change), extensible enums are used to signal to clients that new values may be added to this enum at any time. Clients should be prepared for this and not consider new values to be a breaking change.

Use cases for extensible enums include:
* Values that are only used for display purposes (e.g. in a GUI)
* Values that are not owned by the API and may change due to outside influences

#### Exceptions

None.

