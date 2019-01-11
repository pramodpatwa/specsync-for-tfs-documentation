# `synchronization/areaPath` Configuration

This configuration section contains settings to configure how the test case *area path* field should be updated.

Read more about the setting the *area path* and *iteration path* fields in the [Add new test cases to an Area or an Iteration](add-new-test-cases-to-an-area-or-an-iteration.md) concept description. 

The following example shows the available options within this sub-section.

```
{
  ...
  "synchronization": {
	...
    "areaPath": {
      "mode": "setOnLink",
      "value": "\\MyArea"
    },
	...
  },
  ...
}
```


## Settings

* `mode` -- Specifies how the area path of the test case should be updated. Available options: `notSet` and `setOnLink`. (Default: `notSet`)
  * `notSet`: the path is not set
  * `setOnLink`: set the path when the test case created and linked to the scenario, but not to update later on. 
* `value` -- The area path to set for test cases (e.g. `\\MyArea`). The project name prefix can be omitted.


*[Back to the [`synchronization` Configuration](configuration-synchronization.md)]*

*[Back to the [Configuration guide](../configuration.md)]*