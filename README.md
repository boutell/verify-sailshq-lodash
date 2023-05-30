# verify-sailshq-lodash

* Run `npm install`
* Run `snyk test`
* Note the complaint about `@sailshq/lodash`
* Now try to run `node app`. **It will fail saying that `zipObjectDeep` does not exist.** This is expected because it doesn't.
* But, this is the method that `snyk` says is vulnerable here: [https://security.snyk.io/vuln/SNYK-JS-SAILSHQLODASH-567754](https://security.snyk.io/vuln/SNYK-JS-SAILSHQLODASH-567754)
* Therefore a false positive, unless I am missing something 🤪

Thanks for your time!
