### ID 24 - Use of xxxOf constructs

| Title    | __24 - Use of xxxOf constructs__ |
| :----    | :---------- |
| Strategy | A xxxOf (`allOf`, `anyOf`, oneOf) construct should use a Discriminator. |

<details><summary>

Open section for explanation, rationale and exception conditions 

</summary>

#### Explanation

Although the `allOf`, `anyOf` and `oneOf` constructs are valid OAS3 constructs, they might cause problems when used in combination with older code frameworks. This rule does not forbid the use of these constructs, but merely advises to proceed with caution. 

When `anyOf` or `oneOf` are used in a schema, that schema **should** specify an [OAS Discriminator](https://swagger.io/docs/specification/v3_0/data-models/inheritance-and-polymorphism/) construct to facilitate proper selection between schema variants at run-time.

#### Rationale

In the past, many code generators and applications did not handle the xxxOf constructs properly and generated incorrect code and/or import errors. Today, this situation has improved significantly, making these constructs worth considering for new APIs and for future breaking changes to existing APIs. A market consultation **should** take place beforehand to check whether the market parties can handle the proposed constructs correctly.

#### Exceptions

ASNO does not explicitly mention the use of xxxOf constructs. On the github site of *VNG realisatie* (API working group of the Association of Dutch Municipalities), the recommendation remains to avoid the use of xxxOf. Details can be found at the '[Haal Centraal API design decisions](https://github.com/VNG-Realisatie/Haal-Centraal-common/blob/master/docs/design_decisions.md#dd54-gebruik-geen-oneof-of-anyof-constructies-voor-polymorfe-gegevens)'. 

</details>
