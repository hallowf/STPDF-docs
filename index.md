---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
permalink: /home/
title: titles.home
nav_order: 1
---

<style type="text/css">
.l_list {
    list-style-type: none;
    text-align: center;
    display: flex;
    flex-flow: row wrap;
}
.l_list_items {
    margin: auto;
    text-decoration: none;
}
.l_list_items:hover {
    color: blue;
    text-decoration: none;
    cursor: pointer;
}
</style>
<!-- logo -->
<div style="text-align: center">
    <img style="margin: auto; width: 200px; height: 200px;" src="{{ "/assets/imgs/stpdf-horizontal-win.ico" | prepend: site.baseurl_root}}">
</div>
{: .v-align-middle }

<!-- stpdf -->
{% tf home/stpdf.md %}

<!-- upcoming features -->
{% tf home/up_features.md %}

<!-- features -->
## {% t headers.features %}

### {% t headers.custom_themes %}

<!-- theme immages -->
<img class="themeSlide" src="{{ "/assets/imgs/theme-cmder.png" | prepend: site.baseurl_root }}">
<img class="themeSlide" src="{{ "/assets/imgs/theme-dark.png" | prepend: site.baseurl_root }}">
<img class="themeSlide" src="{{ "/assets/imgs/theme-default.png" | prepend: site.baseurl_root }}">

<!-- script to make carousel of themeSlide images -->
<script>
    var slideIndex = 0;
    carousel();

    function carousel() {
        var i;
        var x = document.getElementsByClassName("themeSlide");
        for (i = 0; i < x.length; i++) {
            x[i].style.display = "none"; 
        }
        slideIndex++;
        if (slideIndex > x.length) {slideIndex = 1} 
        x[slideIndex-1].style.display = "block"; 
        setTimeout(carousel, 2000); // Change image every 2 seconds
    }
</script>

{% tf home/custom_themes.md %}

### {% t headers.deskew %}

<img style="display: inline-block; width:200px; height:300px" src="{{"/assets/imgs/down.png" | prepend: site.baseurl_root}}">
<img style="display: inline-block; width:200px; height:300px" src="{{"/assets/imgs/up.png" | prepend: site.baseurl_root}}">

{% tf home/deskew.md %}

{% tf home/localization.md %}