---
theme: ./
---

# Slidev Theme Smile

Presentation slides for developers

---
layout: intro
hideInToc: true
---

## Summary

<toc minDepth="2"/>

---

## What is Slidev?

Slidev is a slides maker and presenter designed for developers, consist of the following features

- 📝 **Text-based** - focus on the content with Markdown, and then style them later
- 🎨 **Themable** - theme can be shared and used with npm packages
- 🧑‍💻 **Developer Friendly** - code highlighting, live coding with autocompletion
- 🤹 **Interactive** - embedding Vue components to enhance your expressions
- 🎥 **Recording** - built-in recording and camera view
- 📤 **Portable** - export into PDF, PNGs, or even a hostable SPA
- 🛠 **Hackable** - anything possible on a webpage

<br>
<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)


---

## Navigation

Hover on the bottom-left corner to see the navigation's controls panel

### Keyboard Shortcuts

|     |     |
| --- | --- |
| <kbd>space</kbd> / <kbd>tab</kbd> / <kbd>right</kbd> | next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

---
layout: image-right
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
---

## Code

Use code snippets and get the highlighting directly!

```ts
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function editUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = {...user, ...update}  
  saveUser(id, newUser)
}
```

---

## `Alert` component

<alert>This is an info</alert>

<alert type="warning">This is a warning</alert>

<alert type="error">This is an error</alert>

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