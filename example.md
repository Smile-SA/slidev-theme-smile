---
theme: ./
layout: cover
---

# Slidev Theme Smile

Presentation slides for developers

---
layout: intro
---

## Summary

<toc minDepth="2"/>

---
layout: two-cols-with-title
---

## Lists

::left::

Unordered:

* Item 1
* Item 2
  * SubItem 2.1
  * SubItem 2.2
    * SubSubItem 2.2.1
    * SubSubItem 2.2.2
      * SubSubSubItem 2.2.2.1
      * SubSubSubItem 2.2.2.2
        * SubSubSubSubItem 2.2.2.2.1
        * SubSubSubSubItem 2.2.2.2.2
        * SubSubSubSubItem 2.2.2.2.3
      * SubSubSubItem 2.2.2.3
    * SubSubItem 2.2.3
  * SubItem 2.3
* Item 3

::right::

Ordered: 

1. Item 1
2. Item 2
   1. SubItem 2.1
   2. SubItem 2.2
      1. SubSubItem 2.2.1
      2. SubSubItem 2.2.2
         1. SubSubSubItem 2.2.2.1
         2. SubSubSubItem 2.2.2.2
            1. SubSubSubSubItem 2.2.2.2.1
            2. SubSubSubSubItem 2.2.2.2.2
            3. SubSubSubSubItem 2.2.2.2.3
         3. SubSubSubItem 2.2.2.3
      3. SubSubItem 2.2.3
   3. SubItem 2.3
3. Item 3

---

## Table

| Left | Right |
| --- | --- |
| <kbd>space</kbd> / <kbd>tab</kbd> / <kbd>right</kbd> | next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

---
layout: two-cols-demo
---

## Code

::left::

```html
<button class="button" type="button">Click me</button>
<script>
var element = document.querySelector('.button');
function callback(){
  alert('Click!');
};
element.addEventListener('click', callback);
</script>
```

::right::

<button class="button" type="button">Click me</button>
<vScript scoped>
const element = document.querySelector('.button');
function callback(){
  alert('Click!');
};
element.addEventListener('click', callback);
</vScript>

---

## `Alert` component

<alert>This is an `info`</alert>

<alert type="warning">This is a `warning`</alert>

<alert type="error">This is an `error`</alert>

---

## `Icon` and `IconSprite` component

<style>
.slidev-layout p:first-child {
  margin-top: 0;
}

.slidev-layout li {
  line-height: 1em;
}

.slidev-layout li svg {
  font-size: 1.7em;
}
</style>

<icon-sprite/>

<div class="columns-3">

**Filled:**

* **hourglass-filled:** <icon icon="hourglass-filled" />
* **cloud-filled:** <icon icon="cloud-filled" />
* **cart-filled:** <icon icon="cart-filled" />
* **hand-ok-filled:** <icon icon="hand-ok-filled" />
* **cup-filled:** <icon icon="cup-filled" />
* **chess-filled:** <icon icon="chess-filled" />
* **chat-filled:** <icon icon="chat-filled" />
* **lightning-filled:** <icon icon="lightning-filled" />
* **user-filled:** <icon icon="user-filled" />
* **rocket-filled:** <icon icon="rocket-filled" />
* **heart-filled:** <icon icon="heart-filled" />
* **laptop-filled:** <icon icon="laptop-filled" />
* **bulb-filled:** <icon icon="bulb-filled" />
* **gear-filled:** <icon icon="gear-filled" />
* **desktop-filled:** <icon icon="desktop-filled" />

<p class="!mt-4em"><strong>Outlined:</strong></p>

* **smile-confused-outlined:** <icon icon="smile-confused-outlined" />
* **network-outlined:** <icon icon="network-outlined" />
* **smile-eyeglasses-outlined:** <icon icon="smile-eyeglasses-outlined" />
* **chess-outlined:** <icon icon="chess-outlined" />
* **eye-outlined:** <icon icon="eye-outlined" />
* **cloud-1-outlined:** <icon icon="cloud-1-outlined" />
* **padlock-outlined:** <icon icon="padlock-outlined" />
* **target-outlined:** <icon icon="target-outlined" />
* **cloud-2-outlined:** <icon icon="cloud-2-outlined" />
* **100-outlined:** <icon icon="100-outlined" />
* **key-outlined:** <icon icon="key-outlined" />
* **users-outlined:** <icon icon="users-outlined" />
* **chat-outlined:** <icon icon="chat-outlined" />
* **gear-outlined:** <icon icon="gear-outlined" />
* **stars-outlined:** <icon icon="stars-outlined" />
* **smile-heart-outlined:** <icon icon="smile-heart-outlined" />
* **lightning-outlined:** <icon icon="lightning-outlined" />
* **rocket-outlined:** <icon icon="rocket-outlined" />
* **smile-laughing-outlined:** <icon icon="smile-laughing-outlined" />
* **smile-grin-outlined:** <icon icon="smile-grin-outlined" />
* **cart-outlined:** <icon icon="cart-outlined" />
* **bulb-outlined:** <icon icon="bulb-outlined" />
* **desktop-outlined:** <icon icon="desktop-outlined" />
* **bulb-outlined1:** <icon icon="bulb-outlined1" />
* **wave-outlined:** <icon icon="wave-outlined" />
* **hand-victory-outlined:** <icon icon="hand-victory-outlined" />
* **hand-heart-outlined:** <icon icon="hand-heart-outlined" />
* **earth-outlined:** <icon icon="earth-outlined" />
* **smile-outlined:** <icon icon="smile-outlined" />
* **links-outlined:** <icon icon="links-outlined" />
* **hand-ok-outlined:** <icon icon="hand-ok-outlined" />
* **ok-outlined:** <icon icon="ok-outlined" />
* **hand-thumb-up-outlined:** <icon icon="hand-thumb-up-outlined" />
* **check-outlined:** <icon icon="check-outlined" />
* **smile-kiss-outlined:** <icon icon="smile-kiss-outlined" />

</div>

---
layout: center
class: "text-center"
---

## Learn More

[Documentations](https://sli.dev) / [GitHub Repo](https://github.com/slidevjs/slidev)