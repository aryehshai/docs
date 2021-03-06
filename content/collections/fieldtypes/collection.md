---
title: Collection
overview: >
  Allows you attach other Entries to your
  content. Related entries, read-next
  lists, and other useful content
  relationships can all be accomplished
  here.
image: 1ae0abcc-d9c7-412c-8647-fbeedaaa8444
options:
  -
    name: collection
    type: string
    description: >
      The name of the collection to Fetch
      entries from.
id: 0e7eb069-dc0c-4dfd-9230-67ca5d215395
---
## Data Structure {#data-structure}

The Collections fieldtype is a [Relate fieldtype](/docs/fieldtypes/relate), which means the Entries will be saved as IDs.

``` .language-yaml
shows:
  - 892jfsd9a90as
  - 134jk1h78dfas
```

## Templating

Use the [Relate tag](/docs/tags/relate) to loop through the IDs and fetch the content data.

```
<ul>
  {{ relate:shows }}
    <li>{{ title }}</li>
  {{ /relate:shows }}
</ul>
```

``` .language-output
<ul>
  <li>Arrested Development</li>
  <li>Parks and Recreation</li>
</ul>
```
