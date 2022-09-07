# JSON TestCafe Reporter [![npm version](https://img.shields.io/npm/v/testcafe-reporter-cucumber-json.svg)](https://www.npmjs.com/package/testcafe-reporter-cucumber-json-gherkin-testcafe) for gherkin-testcafe based on JSON TestCafé Reporter [![npm version](https://img.shields.io/npm/v/testcafe-reporter-cucumber-json.svg)](https://www.npmjs.com/package/testcafe-reporter-cucumber-json)

This is the **JSON** reporter plugin for [TestCafé](http://devexpress.github.io/testcafe) intergrated with [gherkin-testcafe](https://www.npmjs.com/package/gherkin-testcafe)

This TestCafé reporter generates JSON files that can be merged and converted to a nice and searchable html report by using [multiple-cucumber-html-reporter](https://github.com/wswebcreation/multiple-cucumber-html-reporter).

JSON files generated by this reporter have the same schema than those generated by the Cucumber JSON reporter: this is why `fixture` is translated to `Feature` and `test` to `Scenario` in the final HTML report.

Additionally scenarios contains steps

## To install this TestCafé Reporter

- run the command:

  ```sh
  npm install --save testcafe-reporter-cucumber-json-gherkin-testcafe
  ```

Modification is based on the version 6.3.0 of Look at the JSON TestCafé Reporter, look here https://www.npmjs.com/package/testcafe-reporter-cucumber-json

## Knowlege

TestCafe dynamically loads reporters based on their names. For example, when we set on the command line --reporter foo, TestCafe looks for a folder named testcafe-reporter-foo in the node_modules folder. So in .testcaferc.json configuration should contains reporter name e.g. 
```
 ...
 "reporter": [
        {
            "name": "cucumber-json-gherkin-testcafe",
            "output": "reports/report.json"
        },
 ...
```