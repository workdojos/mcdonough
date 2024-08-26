---
title: Ancestral
headless: true
---


{{ $img := (resources.Get "/images/girl.png").Resize "300x #ccc" }}
{{ $img = $img.Filter (images.Text "Hugo rocks!" (dict
    "color" "#ffffff"
    "size" 60
    "linespacing" 2
    "x" 10
    "y" 20
))}}