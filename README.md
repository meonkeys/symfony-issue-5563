Repro for [symfony issue #5563](https://github.com/symfony/symfony/issues/5563).

# Steps

1. Install dependencies with composer.
1. Run `./repro help foo`

# Expected result

Default URL is displayed without extra escapes.

    Usage:
     foo [-u|--url="..."]
    
    Options:
     --url (-u) A url. (default: "http://example.com/test.txt")

# Actual result

    Usage:
     foo [-u|--url="..."]
    
    Options:
     --url (-u) A url. (default: "http:\/\/example.com\/test.txt")
