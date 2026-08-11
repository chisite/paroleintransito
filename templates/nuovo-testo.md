<%*
const slug = tp.file.title
  .toLowerCase()
  .replace(/[àáâã]/g, "a")
  .replace(/[èéêë]/g, "e")
  .replace(/[ìíîï]/g, "i")
  .replace(/[òóôõ]/g, "o")
  .replace(/[ùúûü]/g, "u")
  .replace(/[^a-z0-9\s-]/g, "")
  .trim()
  .replace(/\s+/g, "-");

tR += `---
title: "${tp.file.title}"
date: ${tp.date.now("YYYY-MM-DD")}
draft: true
slug: "${slug}"
description: ""
tags: []
---

`;
%>
