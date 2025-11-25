---
# You can also start simply with 'default'
theme: academic
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://cover.sli.dev
highlighter: shiki
# some information about your slides (markdown enabled)
title: 11-ECF-hw
info: |
  ICS 2025 Fall Slides
titleTemplate: '%s'
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: fade-out
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
layout: cover
coverBackgroundUrl: /res/image/cover/cover_11.jpg

---

# ECF-HW {.font-bold}

<p class="text-gray-100">
<font size = '5'>
  元培数科 王恩博
</font>
</p>

<div class="pt-12  text-gray-1">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Let's get started <carbon:arrow-right class="inline"/>
  </span>
</div>


<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/WEB-05/WEB-ICS-TA-Slides2025
  " target="_blank" alt="GitHub" title="Open in GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<style>
  div{
   @apply text-gray-2;
  }
</style>



---
layout: center
---

<div>
  <text class="text-17 font-bold gradient-text">Homework Review</text>
</div>

<style>
  .gradient-text {
    background-image: linear-gradient(45deg, #4ec5d4 10%, #146b8c 20%);
    -webkit-background-clip: text;
    color: transparent;
  }
</style>

---

# HW1

![PixPin_2024-11-20_21-39-28](./newres/image/W11/12.png){.w-130}

<div grid="~ cols-2 gap-12">


<div class="text-sm">

| 进程对    | 是否并发 | 
| -------- | ------- | 
| AB     | 否    | 
| AC     | 是    | 
| AD     | 是    | 
| BC     | 是    | 
| BD     | 是    | 
| CD     | 是    | 

</div>
<div>

![PixPin_2024-11-20_21-39-28](./newres/image/W11/13.png){.w-60}

</div>
</div>

---

# HW2


<div grid="~ cols-2 gap-12">


<div class="text-sm">

![PixPin_2024-11-20_21-39-28](./newres/image/W11/14.png){.w-100}

</div>
<div>

![PixPin_2024-11-20_21-39-28](./newres/image/W11/15.png){.w-60}

</div>
</div>

- 排序要求：第一个2前面至少有一个0或1，第二个2前面要至少既有一个0又有一个1。
- 答案：ACE

---

# HW3


![PixPin_2024-11-20_21-39-28](./newres/image/W11/16.png){.w-150}



- 每次循环进程翻一番，执行完循环后打印出的行数就是$2^n$
- 注意上面假设每次当前所有进程都一起执行循环，循环执行完一起打印是为了方便分析的假设，实际上顺序是乱的，但不影响个数。