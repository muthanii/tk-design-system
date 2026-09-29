# FormField

A labelled text field (`.form-group input` in the site's stylesheet): 50px tall, padded 0 × 18px, `radius-4`, a 1px `field-border` outline, 16px text in `text-dark`, with the placeholder in `text`. A textarea (`tk-textarea`) is 160px tall and can be resized vertically.

States:

- **Focus:** a `primary` border with a soft blue ring.
- **Error:** set `aria-invalid="true"`. The border turns `danger`, with a `tk-field__error` message linked by `aria-describedby`.
- **Disabled:** a `surface-alt` fill.

Always put a visible label above the field; placeholders are only hints.

The site's stylesheet outlines fields in `line` (#eee), which is almost invisible (1.2:1). This system uses `field-border` (#8c8c8c, 3.4:1 on white) instead, so fields are easy to spot. That is the one deliberate change from the site's form look.

The site's contact page currently has no form, so these are the stylesheet's field styles plus the states above.
