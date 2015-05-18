# rowlow.layout.vertical-align

This module adds functionality to vertical align not just inline or table elements. A vertical align wrapper in combinations with the ```rowlow.layout.layer-group```module helps you to vertically align things with an unknown height.

You can take control of the vertical alignment for any responsive breakpoint separately.

## Install

```
    bower install --save rowlow.layout.vertical-align
```

## Variables

```
    $rowlow-vertical-align-namespace // Specific module namespace
```


## Usage

### Setup
```
    /* Set modules namespace (optional) */
    $rowlow-vertical-align-namespace: "namespace-";

    @import "bower_components/rowlow.layout.vertical-align/main.scss"
```


### CSS Selector Naming Scheme

```
    .{rowlow-vertical-align-namespace}vertical-align--{breakpoint}--{top, middle, bottom}
    .{rowlow-vertical-align-namespace}vertical-align-helper
```

### HTML
```
    <table>
        <tr>
            <td class="vertical-align--s--top"></td>
            <td class="vertical-align--s--middle"></td>
            <td class="vertical-align--s--bottom"></td>
        </tr>
    </table>


    <div class="vertical-align-helper layer-group" style="height: 200px">
        <div class="vertical-align--s--middle text-align--s--center">
            [...]
        </div>
    </div>
```

