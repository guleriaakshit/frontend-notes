### **What is an Attribute?**

* An **attribute** extends an HTML (or XML) element.
* It can **change the element’s behavior** or **provide extra information/metadata**.

---

# **Attribute Syntax**

* Standard form:
  **`name="value"`**

  * `name` = attribute identifier
  * `value` = the data assigned to it
  * Example: `<img src="cat.png" alt="Cat">`

* Some attributes appear **without `=` or a value** in HTML.

  * This is shorthand for `name=""` (empty string).
  * **Not allowed in XML**, where every attribute must have an explicit value.

---

# **Boolean Attributes**

* Some HTML attributes are **boolean**.
* Their effect depends **only on being present or absent**.
* Examples: `disabled`, `checked`, `required`, `readonly`.

```html
<input type="checkbox" checked>
```

* `checked=""` and `checked` mean the same in HTML.

---

# **Reflection of an Attribute**

* Some attributes are **reflected** as JavaScript **properties** on the corresponding DOM interface.

* This means you can:

  * Read/write them using **JS properties**
    (e.g., `element.id`, `element.value`, `element.disabled`)
  * Or use `getAttribute()` / `setAttribute()`.

* Reflected properties provide a **more natural programming approach** than manually working with attribute methods.
