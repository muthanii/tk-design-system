# Dropdown

The nav submenu (`.header .nav li .dropdown`, under "Our Projects"): a 220px white panel with `shadow-dropdown`, opening below its menu item on hover.

Items are 18px `text-menu` links padded 12px × `space-15`, divided by 1px dashed `line` rules, and turn `primary` on hover or focus. On the site it animates open from 20% height over 0.3s.

The consumer provides the items. It also needs to open on keyboard focus, which the live site does not do (it opens on hover only).
