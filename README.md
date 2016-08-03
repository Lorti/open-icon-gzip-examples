# Open Iconic gzip examples

Should we just inline all SVG icons and stop worrying? What would gzip do?

* `references.html` contains the full [Open Iconic v1.1.1](http://useiconic.com/open) sprite with all 223 SVG icons referenced via `<use>`.
* `inline.html` contains each of the 223 SVG icons inlined in the HTML.
* `duplicates.html` contains each of the 223 SVG icons inlined in the HTML, 10 times in a row.
* `some-duplicates.html` contains each of the 223 SVG icons inlined in the HTML, with 4 icons repeated 20 times.<br>The icons were selected to have different "representative" lengths:
    
        <svg class="icon" width="8" height="8" viewBox="0 0 8 8">
            <path d="M0 0v1h8v-1h-8zm2 2v1h6v-1h-6zm-2 2v1h8v-1h-8zm2 2v1h6v-1h-6z"/>
        </svg>
        <svg class="icon" width="8" height="8" viewBox="0 0 8 8">
            <path d="M1.16 0c-.72.72-1.16 1.71-1.16 2.81s.43 2.12 1.16 2.84l.72-.72c-.54-.54-.88-1.29-.88-2.13 0-.83.33-1.55.88-2.09l-.72-.72zm5.69 0l-.72.72c.54.54.88 1.26.88 2.09 0 .83-.33 1.58-.88 2.13l.72.72c.72-.72 1.16-1.74 1.16-2.84 0-1.1-.43-2.09-1.16-2.81zm-4.25 1.41c-.36.36-.59.86-.59 1.41 0 .55.23 1.08.59 1.44l.69-.72c-.18-.18-.28-.44-.28-.72 0-.28.1-.5.28-.69l-.69-.72zm2.81 0l-.69.72c.18.18.28.41.28.69 0 .28-.1.54-.28.72l.69.72c.36-.36.59-.89.59-1.44 0-.55-.23-1.05-.59-1.41z"
                  transform="translate(0 1)"/>
        </svg>
        <svg class="icon" width="8" height="8" viewBox="0 0 8 8">
            <path d="M2 0c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2zm-1 4.81v3.19l1-1 1 1v-3.19c-.31.11-.65.19-1 .19s-.69-.08-1-.19z"
                  transform="translate(2)"/>
        </svg>
        <svg class="icon" width="8" height="8" viewBox="0 0 8 8">
            <path d="M4 0c-2.2 0-4 1.8-4 4s1.8 4 4 4 4-1.8 4-4-1.8-4-4-4zm0 1c.66 0 1.26.21 1.75.56l-4.19 4.19c-.35-.49-.56-1.09-.56-1.75 0-1.66 1.34-3 3-3zm2.44 1.25c.35.49.56 1.09.56 1.75 0 1.66-1.34 3-3 3-.66 0-1.26-.21-1.75-.56l4.19-4.19z"/>
        </svg>

```
html
 68168 open-iconic-references.html
 59903 open-iconic-inline.html
594522 open-iconic-duplicates.html
 86985 open-iconic-some-duplicates.html

html-gzip-1
 17884 open-iconic-references.html.gz
 14461 open-iconic-inline.html.gz
139610 open-iconic-duplicates.html.gz
 15334 open-iconic-some-duplicates.html.gz

html-gzip-6
 14986 open-iconic-references.html.gz
 11517 open-iconic-inline.html.gz
104971 open-iconic-duplicates.html.gz
 12135 open-iconic-some-duplicates.html.gz

minified
 68167 open-iconic-references.min.html
 59003 open-iconic-inline.min.html
585522 open-iconic-duplicates.min.html
 85525 open-iconic-some-duplicates.min.html

minified-gzip-1
 17888 open-iconic-references.min.html.gz
 14323 open-iconic-inline.min.html.gz
138102 open-iconic-duplicates.min.html.gz
 15213 open-iconic-some-duplicates.min.html.gz

minified-gzip-6
 14990 open-iconic-references.min.html.gz
 11424 open-iconic-inline.min.html.gz
103887 open-iconic-duplicates.min.html.gz
 12029 open-iconic-some-duplicates.min.html.gz
```
