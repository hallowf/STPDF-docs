---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: pages.home
permalink: /
nav_order: 1
---
<div style="text-align: center">
    <img style="margin: auto; width: 200px; height: 200px;" src="{{ "assets/imgs/stpdf-horizontal-win.ico" | prepend: site.baseurl_root}}">
</div>
{: .v-align-middle }

{% tf home/stpdf.md %}

{% tf home/up_features.md %}



## {% t titles.features %}

### {% t titles.custom_themes %}

<img class="themeSlide" src="{{ "assets/imgs/theme-cmder.png" | prepend: site.baseurl_root }}">
<img class="themeSlide" src="{{ "assets/imgs/theme-dark.png" | prepend: site.baseurl_root }}">
<img class="themeSlide" src="{{ "assets/imgs/theme-default.png" | prepend: site.baseurl_root }}">

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


### {% t titles.deskew %}

<img style="display: inline-block; width:200px; height:300px" src="{{"assets/imgs/down.png" | prepend: site.baseurl_root}}">
<img style="display: inline-block; width:200px; height:300px" src="{{"assets/imgs/up.png" | prepend: site.baseurl_root}}">


{% tf home/deskew.md %}


### Localization

This app is currently available in 3 languages:
  * English
  * Portuguese
  * Spanish


if you would like to help with the translation please see [contributing](customization/contributing/)
