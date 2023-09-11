# Partial render file

## Directive that you can use

`partial` or `use`

```
::use{file="/.archbee.yaml" from="1" to="5" syntax="javascript"}
```

## Render petstore from line 9 to 12

::partial{file="../petstore-2.0.yaml#L9-L12"}

## Render .archbee.yaml

::use{file="/.archbee.yaml" from="1" to="5" syntax="javascript"}


## Render file hints.md line 1

### Line 5 only

::partial{file="hints.md#L5"}

### From line 1 to line 5 with lang javascript

::use{file="hints.md" from="5" to="10" syntax="javascript"}


## Print line 2 from .archbee.yaml
::partial{file="/.archbee.yaml#L3"}


## Errors and limitations

### Undefined range

::partial{file="hints.md#L5-L10000"}
### Self referencing is not allowed

The output will not be rendered.

--- 

::partial{file="partial.md#L5"}

___

### Rendering entire file .archbee.yaml is not allowed

::use{file="/.archbee.yaml" syntax="javascript"}