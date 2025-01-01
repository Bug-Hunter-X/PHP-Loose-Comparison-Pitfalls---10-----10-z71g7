# PHP Loose Comparison Bug

This repository demonstrates a common error in PHP related to loose comparison using the `==` operator.  The code compares a string ('10') and an integer (10), showcasing the unexpected result of type juggling.  The solution provides a corrected version using strict comparison (`===`).

## Bug Description

PHP's loose comparison operator (`==`) performs type juggling before comparison, potentially leading to unintended results.  This can be problematic in situations where strict type matching is crucial, such as when working with databases or numerical operations.

## Solution

The solution uses the strict comparison operator (`===`), which requires both the value and the type to be identical for a comparison to evaluate as true. This prevents the type juggling issues encountered with loose comparison and ensures more reliable results.