---
title: "All model fit and calibration options will now be set by default"
date: 2022-09-26
hintr_version: 1.0.41
pull_request: https://github.com/mrc-ide/hintr/pull/405
tags: ["Update"]
---

All model fit and calibration options now have default values. The defaults are the options used in the final naomi fit from last years estimates process. Note that if the value of any of the options used last year is no longer a valid option (for example if the prevalence survey selected last year is not uploaded this year) then we attempt to set a default from information in the input data. This should mean that all countries have an initial set of options for which the model will fit.
