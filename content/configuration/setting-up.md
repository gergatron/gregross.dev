---
title: "Setting up"
order: 1
tocDepth: 1
---

Primary configuration `config.yml` within `config` directory

## Adding images

<Warning>
For adding images (or any other assets) to content, please follow [this](/editing/images) guide instead.
Using assets does not bring performance optimization 
</Warning>

Add images to `static/assets` directory. 
- set a path in `config.yml`  

```yaml
header:
  logo: /assets/logo.png
```

## Using environment variables 

Make use of environment variables (like Algolia API keys) to pass configuration to BooGi / Gatsby while building your project.

Each and every configuration property in `config.yml` can also be
passed in environment variable.

**Important:** List variables are not supported!

**General rule:**

in `config.yml`:
```yaml
property1:
  childProperty: MyApp
```

then env variable should be: `PROPERTY1_CHILD_PROPERTY`.

## Examples

**Example 1:**

<Layout>

```yaml
metadata:
  name: MyApp

features:
  search:
    startComponent: 'input'
```

```bash
METADATA_NAME=MyApp Test
FEATURES_SEARCH_START_COMPONENT=icon
```

</Layout>

**Example 2:**

<Layout>

```yaml
features:
  search:
    enabled: false
```

```bash
FEATURES_SEARCH_ENABLED=true
FEATURES_SEARCH_ALGOLIA_APP_ID=XXXYYYZZZ9
FEATURES_SEARCH_ALGOLIA_SEARCH_KEY=aabbccddeeffgghhiijjkk
FEATURES_SEARCH_ALGOLIA_ADMIN_KEY=xxxyyyzzz
FEATURES_SEARCH_INDEX_NAME=myapp-test-idx
```

</Layout>