# How to set browser specific options in Behave on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=Behave-browser-options)

If you want to set browser specific options for an automation test in Behave on Lambdatest, you can use the following steps. You can refer to sample test repo [here](https://github.com/LambdaTest/Python-Behave-Selenium).

# Steps:

You can specify the various browser specific options in the `conftest.py` file. The following is an example on how to set Chrome specific options using chromeOptions:

 ```python
capabilities = {
        "build": "Sample PY Build",
        "platformName": "Windows 11",
        "browserName": "Chrome",
        "browserVersion": "latest",
        "chromeOptions" : {
                "args" : ["incognito"]  # ChromeOption to start chrome in incognito mode
  }
}
 ```
* The different options available for Chrome can be referred to [here](https://seleniumhq.github.io/selenium/docs/api/py/webdriver_chrome/selenium.webdriver.chrome.options.html).

* For more information you can refer to this LambdaTest [blog](https://www.lambdatest.com/blog/desired-capabilities-in-selenium-testing/?utm_source=github&utm_medium=repo&utm_campaign=Behave-browser-options).

## Run your test

### Running tests through local (linux/unix)
```bash
paver run 
```
###Running tests through local (windows)
```bash
behave features/test.feature 
```

### Running tests through jenkins
```bash
paver run jenkins
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)

