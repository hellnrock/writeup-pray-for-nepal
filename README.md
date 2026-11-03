# writeup-pray-for-nepal

Write-up of Intigriti’s “Pray For Nepal” challenge — DOM Clobbering XSS.

**Live version:** https://labs.hellnrock.com/writeups/pray-for-nepal)

## Summary

The challenge reflects the `person` parameter into the page. A client-side sanitizer removes dangerous tags and event handlers, but leaves `id` and `data-*` attributes. By injecting two specific elements, the client-side gate is satisfied and loads a same-origin script that triggers the overridden `alert`, disclosing the flag.

## Flag

`INTIGRITI{f2cb05a5-5cc1-4d1d-b7cd-084306cbd5a0}`

## Structure

```
/
├── index.html
└── images/
    ├── pray-for-nepal-original-network.png
    ├── Payload.png
    ├── intigriti-pray-for-nepal-archive-open.png
    └── pray-for-nepal-flag.png
```

---

HNR Labs · [labs.hellnrock.com](https://labs.hellnrock.com)
