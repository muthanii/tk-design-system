# MobileMenu

The site's header below 768px (SlickNav):

- **Top bar:** centred, with About and Contact on one line and the phone and email below.
- **Logo:** the company logo at full width, up to 310px (about 88px tall).
- **Menu button:** a transparent, right-aligned button of three 25×3px `primary` bars with 1px corners.
- **Open menu:** a plain white list of 14px `ink` links padded 4px × 10px, with no dividers. "Our Projects" carries a small ► and expands its submenu, indented in `text-menu`. The Arabic switch sits last as a small primary button.

The consumer provides the items. The button needs `aria-expanded` to reflect whether the menu is open.

Flags against the live page:

- The current page isn't marked in the mobile menu. Set `aria-current="page"` on it, and style it `primary` if a visible marker is wanted.
- The menu button's tap area is only 25×14px. Pad it to at least 44×44px without changing how it looks.
