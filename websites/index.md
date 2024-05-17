---
title: Websites
layout: fetch
fetch_url: https://cdn.jsdelivr.net/gh/langnang/storage/json/websites.json
---
> 网站

<ul>
  <li v-for="(content,index) in fetch.data.contents" v-bind:key="index" v-text="content.title"></li>
</ul>

<script>
  $(document).ready(()=>{
    console.log(app);
  })
</script>
