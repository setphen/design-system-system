---
title: "{{ replace .Name "-" " " | title }}"
desc:
  A description of the component
variants:
  - name: Component variant
    src: component
    classes: [{{ replace .Name "-" " " }}]
    desc:
      A variant description.

---

