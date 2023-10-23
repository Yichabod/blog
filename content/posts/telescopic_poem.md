---
title: "Ostrom's Teachings"
date: 2022-2-18
draft: false
---
<div id="text-container"></div>

<script>
    const content = `
* I 
  * Yawning, I
    * Yawning, Yawning, Yawning
        * I saw her
* made 
* tea
    * love`;
    const node = createTelescopicTextFromBulletedList(content);
    const container = document.getElementById("text-container");
    container.appendChild(node);
</script>