# scrapy-playwright changelog

### [v0.0.26](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.26) (2023-02-01)

* Fix logging (pass extra args instead of updating log record factory)
* Miscellaneous adjustments (naming, typing, etc)


### [v0.0.25](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.25) (2023-01-24)

* Set spider attribute on log records


### [v0.0.24](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.24) (2022-12-04)

* Fix request method override


### [v0.0.23](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.23) (2022-11-27)

* Set redirect request metadata


### [v0.0.22](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.22) (2022-10-09)

* Remove deprecated code (`PageCoroutine` class, `playwright_page_coroutines` request meta key,
  `use_playwright_headers` function).
* `playwright_page_init_callback` meta key (page initialization callback)


### [v0.0.21](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.21) (2022-08-08)

* Fixed TypeError exception when getting server IP address


### [v0.0.20](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.20) (2022-08-03)

* Don't raise exceptions if `Page.goto` returns `None`


### [v0.0.19](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.19) (2022-07-17)

* Add support for `Page.goto` keyword arguments (`playwright_page_goto_kwargs` request meta key)


### [v0.0.18](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.18) (2022-06-18)

* Always override request headers


### [v0.0.17](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.17) (2022-05-22)

* Support for persistent contexts
* Limit concurrent context count (`PLAYWRIGHT_MAX_CONTEXTS` setting)


### [v0.0.16](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.16) (2022-05-14)

* Use new headers API introduced in Playwright 1.15 (bump required Playwright version)
* Deprecate `scrapy_playwright.headers.use_playwright_headers`, set `PLAYWRIGHT_PROCESS_REQUEST_HEADERS=None` instead


### [v0.0.15](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.15) (2022-05-08)

* Remove deprecated `PLAYWRIGHT_CONTEXT_ARGS` setting
* Warn on failed requests
* `PLAYWRIGHT_ABORT_REQUEST` setting: accept coroutine functions
* `PLAYWRIGHT_PROCESS_REQUEST_HEADERS` setting: accept sync functions to process headers
* Set `playwright_page` request meta key early


### [v0.0.14](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.14) (2022-03-26)

* Renamed `scrapy_playwright.page.PageCoroutine` to `scrapy_playwright.page.PageMethod`
  (`PageCoroutine` is now deprecated). Also deprecated the `playwright_page_coroutines`
  Request meta key in favor of `playwright_page_methods`.


### [v0.0.13](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.13) (2022-03-24)

* PageCoroutine checks
* Fix encoding detection
* Ability to abort requests via setting


### [v0.0.12](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.12) (2022-03-15)

* Avoid exceptions during cleanup when the browser could not start
* Warn when non PageCoroutine objects are passed to Request.meta.playwright_page_coroutines


### [v0.0.11](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.11) (2022-03-12)

* Set the maximum amount of pages per context
* Response.ip_address attribute
* Response security details


### [v0.0.10](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.10) (2022-03-02)

* Fix response encoding detection


### [v0.0.9](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.9) (2022-01-27)

* Ability to process request headers


### [v0.0.8](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.8) (2022-01-13)

* Fix PLAYWRIGHT_DEFAULT_NAVIGATION_TIMEOUT setting (allow zero value)


### [v0.0.7](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.7) (2021-10-20)

* Log all requests/responses (debug level)


### [v0.0.6](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.6) (2021-10-19)

* Page event handlers
* Python 3.10 support
* Doc fixes
* Override User-Agent header


### [v0.0.5](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.5) (2021-08-20)

* Improve garbage collection by removing unnecessary reference

### [v0.0.4](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.4) (2021-07-16)

* Add support for multiple browser contexts ([#13](https://github.com/scrapy-plugins/scrapy-playwright/pull/13))
* Deprecate `PLAYWRIGHT_CONTEXT_ARGS` setting in favor of `PLAYWRIGHT_CONTEXTS`


### [v0.0.3](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.3) (2021-02-22)

* Snake case (requires playwright-python >= [v1.8.0a1](https://github.com/microsoft/playwright-python/releases/tag/v1.8.0a1))


### [v0.0.2](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.2) (2021-01-13)

* `PLAYWRIGHT_CONTEXT_ARGS` setting (ability to pass keyword arguments to the browser context)

### [v0.0.1](https://github.com/scrapy-plugins/scrapy-playwright/releases/tag/v0.0.1) (2020-12-18)

Initial public release.
