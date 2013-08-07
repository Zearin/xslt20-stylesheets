# Notes


## Naming Conventions

Named templates have hyphens (`-`), not periods (`.`).

Namespaces are as follows:

 - **Modes:** `xmlns:m="http://docbook.org/xslt/ns/mode"`
 - **Private modes:** `xmlns:mp="http://docbook.org/xslt/ns/mode/private"`

 - **Functions:** `xmlns:f="http://docbook.org/xslt/ns/extension"`
 - **Private functions:** `xmlns:fp="http://docbook.org/xslt/ns/extension/private"`

 - **Templates:** `xmlns:t="http://docbook.org/xslt/ns/template"`
 - **Private templates:** `xmlns:tp="http://docbook.org/xslt/ns/template/private"`


## About Tools

 - `tools/doccheck.xsl`: checks for documentation problems
 - `tools/writetests`: runs the unit tests:
    1. **Process `html/docbook.xsl` with `tools/writetests.xsl` using _Saxon 8b_. (You need 8.4 patched.)** 
       This will produce the stylesheet `tests.xsl`
    2. **Process `tests.xsl` with any input you want.** 
       This will produce an HTML summary of the unit tests.


## Miscellaneous

- [ ] Consider making `<index/>` contextual, so an index in a `<part/>` (for example) can index just that part.


