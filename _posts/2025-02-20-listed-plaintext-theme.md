---
tags: internet
title: Listed.to plaintext theme
---

![a listed.to blog but it looks like a plaintext site!](/assets/images/post-images/listed-to-plaintext.png)

have you ever wanted to use listed.to as your blog but you want it to look like one of those plaintext only sites? me neither, actually.

so here's how _you_ can do it to!

## getting custom css on listed.to

1. setup a listed.to blog through Standard Notes
2. go to settings > general tab > apperance section > tick 'enable custom css', and save changes
3. create a new note
   1. you can name it whatever you want, but call it something like `style.css` to avoid confusion
   2. put the `metatype: css` yaml frontmatter
   3. start writing (or copying) some css!
   4. publish the note like it's a regular post! it won't get published as a post, i promise.... _if_ you do it right.

yeag... it's a bit janky isn't it?

## the css

### what is this?

i just copied listed.to's css and set everything to revert, essentially removing the style. to no one's surprise, the site now looks ugly as some of the styles are actually essential. luckily this works out cause the more stuff you hide the most plaintext it looks and i just hid everything.

### what does it look like?

[https://listed.to/@meow_d](https://listed.to/@meow_d)

### ok stop teasing me and just give me the css

okay.... here you go....

```css
---
metatype: css
---

/* reset everything */
.error-toast__container {
  position: revert;
  top: revert;
  left: revert;
  width: revert;
  display: revert;
  justify-content: revert;
  transition: revert;
}

.error-toast__toast {
  margin: revert;
  background-color: revert;
  padding: revert;
  display: revert;
  justify-content: revert;
  align-items: revert;
  border-radius: revert;
  border: revert;
}

.error-toast .error-toast__message {
  margin-right: revert;
}

.error-toast .error-toast__dismiss-button {
  padding: revert;
  line-height: revert;
}

.error-toast .error-toast__dismiss-button path {
  fill: revert;
}

.error-toast--visible .error-toast__container {
  top: revert;
}

.pages-menu .page-link {
  color: revert;
}

.pages-menu .page-link.button--no-fill {
  background-color: revert;
  position: revert;
}

.pages-menu .page-link.button--no-fill:before {
  background-image: revert;
  opacity revert;
}

.pages-menu .page-link.button--no-fill:hover {
  color: revert;
}

.pages-menu .page-link.button--active:before {
  background-color: revert;
  opacity revert;
}

.pages-menu__container {
  overflow: revert;
}

.pages-menu--mobile {
  display: revert;
  flex-direction: revert;
  text-align: revert;
  padding: revert;
  visibility: revert;
  margin-top: revert;
  transition: revert;
}

.pages-menu--mobile .button {
  width: revert;
}

.pages-menu--mobile .button:not(:last-child) {
  margin-bottom: revert;
}

.pages-menu--mobile .button.button--primary {
  margin-bottom: revert;
}

.pages-menu--mobile.pages-menu--mobile-visible {
  visibility: revert;
  margin-top: revert;
}

@media (min-width:992px) {
  .pages-menu--mobile {
    display: revert;
  }
}
.pages-menu--desktop {
  display: revert;
}

@media (min-width:992px) {
  .pages-menu--desktop {
    display: revert;
    align-items:flex-start
  }
  .pages-menu--desktop .button {
    margin-left:8px
  }
  .pages-menu--desktop .button.button--primary {
    margin-left: revert;
  }
}
.header-author-info {
  padding: revert;
  text-align: revert;
  border-bottom: revert;
  overflow: revert;
}

.header-author-info .word-count__button {
  padding: revert;
  position: revert;
  min-width: revert;
}

.header-author-info .word-count__button:before {
  content: revert;
  position: revert;
  top: revert;
  right: revert;
  bottom: revert;
  left: revert;
  opacity: revert;
  border-radius: revert;
  min-height: revert;
  min-width: revert;
  background-image: revert;
  transition: revert;
}

@media (min-width:992px) {
  .header-author-info .word-count__button {
    padding:56px 22vw
  }
  .header-author-info .word-count__button:hover:before {
    top: revert;
    opacity: revert;
  }
}
.header-author-info .word-count__button .word-count {
  color: revert;
  font-weight: revert;
  margin-bottom: revert;
}

.header-author-info .word-count__button .word-count__icon {
  display: revert;
  margin: revert;
  height: revert;
  width: revert;
  transform: revert;
}

.header-author-info .word-count__button .word-count__icon path {
  fill: revert;
}

@media (min-width:992px) {
  .header-author-info {
    padding: revert;
  }
}
.author-link {
  color: revert;
}

.author-link:before {
  background-image: revert;
}

.author-twitter {
  color: revert;
}

.author-twitter:before {
  background-image: revert;
}

.bio {
  color: revert;
  white-space: revert;
  font-weight: revert;
}

.header-author-info__items {
  margin-bottom: revert;
  min-height: revert;
  display: revert;
  flex-direction: revert;
  justify-content: revert;
  transition: revert;
}

@media (min-width:992px) {
  .header-author-info__items {
    min-height: revert;
    flex-direction: revert;
    align-items: revert;
    justify-content: revert;
    text-align: revert;
    margin-bottom: revert;
  }
}
.header-image-container {
  width: revert;
  height: revert;
  display: revert;
  justify-content: revert;
  align-items: revert;
  margin-bottom: revert;
  border-radius: revert;
  overflow: revert;
  position: revert;
}

.header-image-container:before {
  content: revert;
  position: revert;
  top: revert;
  right: revert;
  bottom: revert;
  left: revert;
  background-color: revert;
  opacity revert;
}

@media (min-width:992px) {
  .header-image-container {
    width: revert;
    min-width: revert;
    height: revert;
    margin-right: revert;
    margin-bottom: revert;
  }
}
.header-image {
  height: revert;
  width: revert;
  background-size: revert;
  background-position: revert;
}

.header-author-capital {
  color: revert;
  opacity: revert;
  font-size: revert;
  font-family: revert;
}

.p1.bio {
  margin-top: revert;
}

@media (min-width:992px) {
  .p1.bio {
    margin-top: revert;
  }
}
.p2.header-author-links {
  margin-top: revert;
}

.p2.header-author-links .item:not(:last-of-type):after {
  content: revert;
  color: revert;
  padding: revert;
}

.page-header__container {
  padding-top: revert;
}

@media (min-width:992px) {
  .page-header__container {
    padding-top: revert;
  }
}
.page-header__container .listed-logo-link {
  display: revert;
  padding: revert;
  margin: revert;
  color: revert;
}

.page-header__container .listed-logo-link.button--no-fill {
  background-color: revert;
  position: revert;
}

.page-header__container .listed-logo-link.button--no-fill:before {
  background-image: revert;
  opacity revert;
}

.page-header__container .listed-logo-link.button--no-fill:hover {
  color: revert;
}

.page-header__container .listed-logo-link .listed-logo__animated path {
  animation: revert;
  fill: revert;
}

.page-header__container .listed-logo-link:before {
  background-image: revert;
}

@media (min-width:992px) {
  .page-header__container .listed-logo-link {
    padding: revert;
  }
}
.page-header__container--post {
  background-color: revert;
}

#page-header {
  width: revert;
  padding: revert;
  display: revert;
  justify-content: revert;
  align-items: revert;
}

@media (min-width:992px) {
  #page-header {
    padding: revert;
  }
}
.left {
  display: revert;
}

@media (min-width:992px) {
  .website-name {
    padding: revert;
  }
}
.listed-logo {
  height: revert;
  width: revert;
}

@media (min-width:992px) {
  .listed-logo {
    height: revert;
    width: revert;
  }
}
@keyframes changeColor {
  0% {
    fill:var(--color-primary)
  }
  to {
    fill: revert;
  }
}
.author-name__container {
  display: revert;
}

.author-name__container:before {
  content: revert;
  color: revert;
  opacity: revert;
  margin: revert;
  font-size: revert;
  line-height: revert;
}

@media (min-width:992px) {
  .author-name__container:before {
    margin: revert;
  }
}
.author-name__container .author-name.path-item {
  display: revert;
  align-items: revert;
}

.author-name__container .author-name.path-item a {
  color: revert;
  padding: revert;
  margin: revert;
}

.author-name__container .author-name.path-item a.button--no-fill {
  background-color: revert;
  position: revert;
}

.author-name__container .author-name.path-item a.button--no-fill:before {
  background-image: revert;
  opacity revert;
}

.author-name__container .author-name.path-item a.button--no-fill:hover {
  color: revert;
}

.author-name__container .author-name.path-item a:before {
  background-image: revert;
}

@media (min-width:992px) {
  .author-name__container .author-name.path-item a {
    padding: revert;
  }
}
.right {
  display: revert;
}

.button.button--menu-icon {
  height: revert;
  width: revert;
  padding: revert;
  background: revert;
}

.button.button--menu-icon svg path {
  fill: revert;
}

@media (min-width:992px) {
  .button.button--menu-icon {
    display: revert;
  }
}
.left-nav-bar {
  display: revert;
  width: revert;
  height: revert;
  margin-right: revert;
  position: revert;
  top: revert;
}

.left-nav-bar .button {
  width: revert;
  text-align: revert;
  display: revert;
  align-items: revert;
}

.left-nav-bar .button:before {
  transition: revert;
}

.left-nav-bar .button:not(.button--active) {
  color: revert;
}

.left-nav-bar .button:not(.button--active) svg path {
  fill: revert;
}

.left-nav-bar .button:not(:last-child) {
  margin-bottom: revert;
}

.left-nav-bar .button--active .left-nav-bar__icon path {
  fill: revert;
}

@media (min-width:992px) {
  .left-nav-bar {
    display: revert;
  }
}
.left-nav-bar__icon {
  margin-right: revert;
}

.section__container {
  list-style-type: revert;
}

.section__container:not(:last-child) {
  margin-bottom: revert;
}

@media (min-width:992px) {
  .section__container:not(:last-child) {
    margin-bottom: revert;
  }
}
.card.section--desktop {
  display: revert;
  padding: revert;
}

@media (min-width:992px) {
  .card.section--desktop {
    display: revert;
  }
}
@media (min-width:992px) {
  .section--mobile {
    display: revert;
  }
}
.section__headline {
  display: revert;
  align-items: revert;
}

.section__collapse-icon {
  margin-left: revert;
}

.section__collapse-icon path {
  fill: revert;
}

.section__content {
  max-height: revert;
  visibility: revert;
  overflow: revert;
  transition: revert;
}

.left-nav-bar-page__header {
  margin-bottom: revert;
}

.left-nav-bar-page__header .p1 {
  margin-top: revert;
}

.left-nav-bar-page__content {
  display: revert;
}

.left-nav-bar-page__sections {
  width: revert;
  margin: revert;
  padding: revert;
}

.form-section.checkbox__container {
  flex-direction: revert;
}

.checkbox {
  display: revert;
}

.checkbox__icon-container {
  margin-right: revert;
  height: revert;
  width: revert;
}

.checkbox__icon-container svg path {
  fill: revert;
}

.confirmation-modal__overlay {
  position: revert;
  background-color: revert;
  width: revert;
  height: revert;
  top: revert;
  left: revert;
  display: revert;
  flex-direction: revert;
  justify-content: revert;
  z-index: revert;
}

.confirmation-modal__modal {
  margin: revert;
}

@media (min-width:992px) {
  .confirmation-modal__modal {
    margin: revert;
  }
}
.confirmation-modal__buttons {
  margin-top: revert;
  display: revert;
  justify-content: revert;
}

.confirmation-modal__buttons .button--primary {
  margin-left: revert;
  background-image: revert;
}

.confirmation-modal__buttons .button--no-fill {
  color: revert;
}

.confirmation-modal__buttons .button--no-fill.button--no-fill {
  background-color: revert;
  position: revert;
}

.confirmation-modal__buttons .button--no-fill.button--no-fill:before {
  background-image: revert;
  opacity revert;
}

.confirmation-modal__buttons .button--no-fill.button--no-fill:hover {
  color: revert;
}

.confirmation-modal__buttons .button--secondary-disabled {
  color: revert;
}

.dropdown {
  position: revert;
}

.dropdown .button {
  margin: revert;
  padding: revert;
  font-weight: revert;
}

.dropdown__list.card {
  z-index: revert;
  opacity: revert;
  visibility: revert;
  position: revert;
  right: revert;
  margin: revert;
  padding: revert;
  list-style: revert;
  width: revert;
  background-image: revert;
  transition: revert;
}

.dropdown__list.card.dropdown__list--open {
  opacity: revert;
  visibility: revert;
  box-shadow: revert;
}

.dropdown__option {
  padding: revert;
}

.dropdown__option:not(:last-child) {
  margin-bottom: revert;
}

.dropdown__option:hover {
  background-color: revert;
}

.dropdown__option .option__button {
  width: revert;
  text-align: revert;
  display: revert;
  align-items: revert;
}

.dropdown__option .option__icon {
  margin-right: revert;
  width: revert;
  height: revert;
}

.dropdown__option .option__icon path {
  fill: revert;
}

.my-posts {
  padding: revert;
  margin: revert;
  list-style-type: revert;
}

.my-posts__item {
  padding: revert;
  border-top: revert;
  display: revert;
  align-items: revert;
}

.my-posts__item:last-child {
  border-bottom: revert;
}

.my-posts__item a.my-posts__post {
  color: revert;
  flex-grow: revert;
}

.my-posts__item a.my-posts__post:before,
.my-posts__item a.my-posts__post:hover:before {
  background-image: revert;
}

.my-posts__item a.my-posts__post .post__details {
  color: revert;
  font-weight: revert;
  display: revert;
  align-items: revert;
  margin-top: revert;
}

.my-posts__item a.my-posts__post .post__details .post-details__icon {
  width: revert;
  height: revert;
  margin-right: revert;
}

.my-posts__item a.my-posts__post .post__details .post-details__icon path {
  fill: revert;
}

.my-posts__item a.my-posts__post .post-details__item {
  display: revert;
  align-items: revert;
}

.my-posts__item a.my-posts__post .post-details__item:not(:last-child):after {
  content: revert;
  margin: revert;
}

.guestbook-entries {
  padding: revert;
  margin: revert;
  list-style-type: revert;
}

.guestbook-entries__item {
  padding: revert;
  border-top: revert;
  display: revert;
  align-items: revert;
}

.guestbook-entries__item:last-child {
  border-bottom: revert;
}

.guestbook-entries__item .button--make-public {
  display: revert;
}

@media (min-width:992px) {
  .guestbook-entries__item .button--make-public {
    display: revert;
    margin-right: revert;
  }
}
.guestbook-entries__entry {
  flex-grow: revert;
}

.guestbook-entries__entry .entry__details {
  color: revert;
  font-weight: revert;
  display: revert;
  align-items: revert;
  margin-top: revert;
}

.guestbook-entries__entry .entry__details--private {
  display: revert;
}

.guestbook-entries__entry .entry__details .entry-details__icon {
  width: revert;
  height: revert;
  margin-right: revert;
}

.guestbook-entries__entry .entry__details .entry-details__icon path {
  fill: revert;
}

.guestbook-entries__entry .entry-details__item {
  display: revert;
  align-items: revert;
}

.guestbook-entries__entry .entry-details__item:not(:last-child):after {
  content: revert;
  margin: revert;
}

@media (min-width:992px) {
  .guestbook-entries__action--make-public {
    display: revert;
  }
}
.custom-domain .form-row {
  align-items: revert;
}

.custom-domain .form-row--error .form-section {
  padding-top: revert;
}

.custom-domain .callout {
  margin-top: revert;
  width: revert;
}

.custom-domain .hover-container {
  display: revert;
  align-items: revert;
  min-height: revert;
}

.custom-domain .custom-domain__info {
  margin-top: revert;
}

.custom-domain__details {
  display: revert;
  flex-wrap: revert;
  align-items: revert;
  flex-grow: revert;
}

.custom-domain__linked-icon {
  height: revert;
  width: revert;
  margin-right: revert;
}

.credential-form .form-row {
  align-items: revert;
}

.payment-details .payment-details__info {
  margin-top: revert;
}

.payment-details .callout {
  margin-top: revert;
  width: revert;
}

.payment-details .callout:first-child {
  margin-top: revert;
}

.payment-details .payment-details__credential {
  color: revert;
  font-weight: revert;
  display: revert;
  align-items: revert;
  min-height: revert;
}

.payment-details .credential__details {
  display: revert;
  flex-wrap: revert;
  align-items: revert;
  flex-grow: revert;
}

.payment-details .credential__details svg path {
  fill: revert;
}

.payment-details .credential__key:not(:last-child):after {
  content: revert;
  margin: revert;
}

.payment-details .credential__icon {
  height: revert;
  width: revert;
  margin-right: revert;
}

.delete-blog .delete-blog__info {
  margin-top: revert;
}

.delete-blog .delete-blog__instructions {
  font-weight: revert;
  margin-top: revert;
}

.delete-blog .delete-blog__button-container {
  display: revert;
}

.delete-blog__button {
  margin-top: revert;
  width: revert;
}

.delete-blog__button.button--primary {
  background-image: revert;
}

@media (min-width:992px) {
  .delete-blog__button {
    width: revert;
  }
}
.delete-blog__form .checkbox__container--checked {
  color revert;
}

.delete-blog__form .checkbox__container--checked .checkbox__icon-container svg path {
  fill revert;
}

.form-section.radio-button__container {
  border: revert;
  border-radius: revert;
  height: revert;
  width: revert;
  padding: revert;
  margin-right: revert;
  cursor: revert;
}

.radio-button__svg-container {
  height: revert;
  overflow: revert;
  border-top-right-radius: revert;
  border-top-left-radius: revert;
}

.radio-button__svg-container .svg-background {
  fill: revert;
}

.radio-button__svg-container .svg-items {
  fill: revert;
}

.radio-button__image-container img {
  height: revert;
  width: revert;
}

.radio-button {
  display: revert;
}

.radio-button__icon-container {
  margin-right: revert;
  height: revert;
  width: revert;
}

.radio-button__icon-container svg path {
  fill: revert;
}

.radio-button__input-container {
  display: revert;
  padding: revert;
  align-items: revert;
  justify-content: revert;
  border-top: revert;
}

.form-section.radio-button-group__options-container {
  flex-direction: revert;
  padding-top: revert;
}

#resources .resources__list {
  margin: revert;
  padding: revert;
  list-style-type: revert;
}

#resources .resources__list li {
  border-bottom: revert;
}

#resources .resources__list li:first-child {
  border-top: revert;
}

#resources .resources__list li a {
  font-weight: revert;
  color: revert;
  padding: revert;
  display: revert;
  align-items: revert;
  justify-content: revert;
  text-align: revert;
}

#resources .resources__list li a:hover {
  padding: revert;
}

#resources .resources__link:before,
#resources .resources__link:hover #resources .resources__link:before {
  background-image: revert;
}

.resources__hover-content {
  display: revert;
}

.accessible-via {
  list-style-type: revert;
  margin: revert;
  padding: revert;
}

.post-content .post-header .post-title {
  color: revert;
  word-wrap: revert;
}

.post-content .post-header .post-title a:before {
  background-image: revert;
}

.post-content .post-body {
  margin: revert;
  word-wrap: revert;
}

.post-content .post-body h1 {
  font-size: revert;
}

.post-content .post-body h2 {
  font-size: revert;
}

.post-content .post-body h3 {
  font-size: revert;
}

.post-content .post-body h4 {
  font-size: revert;
}

.post-content .post-body h5 {
  font-size: revert;
}

.post-content .post-body h6 {
  font-size: revert;
}

.post-content .post-body li:not(:last-child) {
  margin-bottom: revert;
}

.post-content .post-body p:not(:last-child) {
  margin-bottom: revert;
}

.post-content .post-body pre {
  padding: revert;
  overflow: revert;
  font-size: revert;
  background-color: revert;
}

.post-content .post-body p code {
  font-family: revert;
  font-size: revert;
  padding: revert;
  background-color: revert;
  border: revert;
  border-radius: revert;
}

.post-content .post-body img {
  display: revert;
  margin-top: revert;
  max-width: revert;
}

.post-content .post-body table {
  display: revert;
  width: revert;
  overflow: revert;
  border-collapse: revert;
  border-spacing: revert;
  border-color: revert;
}

.post-content .post-body table td,
.post-content .post-body table th {
  padding: revert;
  border: revert;
}

.post-content .post-body table tr:nth-child(2n) {
  background-color: revert;
}

.post-content .post-date {
  margin-top: revert;
  opacity revert;
}

.post-content .post-date__separator {
  margin: revert;
}

.author-post .read-more-link {
  margin-top: revert;
}

.post-preview {
  height: revert;
  display: revert;
  flex-direction: revert;
}

.post-preview .post-body {
  margin: revert;
}

.post-preview .post-body p:not(:last-child) {
  margin-bottom: revert;
}

.post-preview .post-body,
.post-preview.post-content a .post-header {
  color: revert;
  font-weight: revert;
}

.post-preview .read-more-link {
  background: revert;
  display: revert;
}

.post-preview .read-more-link:hover {
  background: revert;
}

.post-preview .read-more-link:hover .read-more-link__icon path {
  fill: revert;
}

.post-preview .read-more-link:before {
  content: revert;
}

.post-preview .read-more-link__icon {
  width: revert;
  height: revert;
  margin-left: revert;
}

.post-preview .read-more-link__icon path {
  fill: revert;
}

.button.scroll-to-top__button {
  background-color: revert;
  position: revert;
  bottom: revert;
  right: revert;
  padding: revert;
  border-radius: revert;
  display: revert;
}

.button.scroll-to-top__button .scroll-to-top__container {
  width: revert;
  height: revert;
  border: revert;
  border-radius: revert;
  background-color: revert;
  display: revert;
  align-items: revert;
  justify-content: revert;
  opacity: revert;
  transition: revert;
}

.button.scroll-to-top__button .scroll-to-top__container .scroll-to-top__icon {
  width: revert;
  height: revert;
  transform: revert;
}

.button.scroll-to-top__button .scroll-to-top__container .scroll-to-top__icon path {
  fill: revert;
}

.button.scroll-to-top__button .scroll-to-top__container:hover {
  border: revert;
}

.button.scroll-to-top__button--visible {
  display: revert;
}

.button.scroll-to-top__button--visible .scroll-to-top__container {
  opacity: revert;
}

#author-all {
  padding: revert;
}

@media (min-width:992px) {
  #author-all {
    padding: revert;
  }
}
#author-profile {
  padding: revert;
  background-color: revert;
}

#author-profile .older {
  padding: revert;
  display: revert;
  justify-content: revert;
}

#author-profile .older button {
  color: revert;
  display: revert;
}

#author-profile .older button svg {
  margin-left: revert;
}

#author-profile .older button svg path {
  fill: revert;
}

@media (min-width:992px) {
  #author-profile .older {
    padding: revert;
  }
}
@media (min-width:992px) {
  #author-profile {
    padding: revert;
  }
}
.author-post {
  padding: revert;
}

.author-post:not(:last-child) {
  border-bottom: revert;
}

@media (min-width:992px) {
  .author-post {
    padding: revert;
  }
}
@media (min-width:1400px) {
  .author-post {
    padding: revert;
  }
}
#subscription-form .text-field {
  width: revert;
  margin: revert;
}

@media (min-width:992px) {
  #subscription-form .text-field {
    width: revert;
    margin-bottom: revert;
  }
}
#subscription-form .button {
  width: revert;
}

@media (min-width:992px) {
  #subscription-form .button {
    width: revert;
  }
}
#subscribe-page .h1 {
  margin-bottom: revert;
}

#subscribe-page #subscription-form {
  margin: revert;
}

#subscribe-page .subscribe-page__rss-feed {
  text-align: revert;
}

@media (min-width:992px) {
  #subscribe-page .subscribe-page__rss-feed {
    text-align: revert;
  }
}
#tip .h1,
#tip .p1 {
  margin-bottom: revert;
}

#tip .tip__credentials {
  margin-top: revert;
}

#tip .callout {
  width: revert;
}

#tip .callout:not(:last-child) {
  margin-bottom: revert;
}

.guestbook-entry-form__container {
  display: revert;
  margin: revert;
}

.guestbook-entry-form__button-container {
  margin-top: revert;
}

.guestbook-entry-form__button-container .button {
  width: revert;
  margin-bottom: revert;
}

@media (min-width:992px) {
  .guestbook-entry-form__button-container {
    display: revert;
    align-items:center
  }
  .guestbook-entry-form__button-container .button {
    width: revert;
    margin: revert;
  }
}
.guestbook-entry-form__error-message {
  color: revert;
  margin-top: revert;
}

.guestbook__container .callout {
  margin: revert;
}

.guestbook__new-entry-button-container {
  display: revert;
  flex-direction: revert;
  margin: revert;
}

.guestbook__new-entry-button-container .p1 {
  margin-bottom: revert;
}

@media (min-width:992px) {
  .guestbook__new-entry-button-container {
    flex-direction: revert;
    align-items: revert;
    margin-top:24px
  }
  .guestbook__new-entry-button-container .button {
    margin-right:16px
  }
  .guestbook__new-entry-button-container .p1 {
    margin-bottom: revert;
  }
}
.guestbook__entry {
  border-left: revert;
  border-radius: revert;
  padding-left: revert;
}

.guestbook__entry:not(:last-child) {
  margin-bottom: revert;
}

.single-post-show {
  padding: revert;
  background-color: revert;
}

.single-post-show hr {
  margin-bottom: revert;
}

.single-post-show .post-content {
  padding: revert;
}

@media (min-width:992px) {
  .single-post-show .post-content {
    padding: revert;
  }
}
@media (min-width:1400px) {
  .single-post-show .post-content {
    padding: revert;
  }
}
.single-post-show #subscription-form {
  text-align: revert;
}

.single-post-show #subscription-form .callout,
.single-post-show #subscription-form .sublabel {
  margin: revert;
}

@media (min-width:992px) {
  .single-post-show {
    padding: revert;
  }
}
.more-from {
  display: revert;
  align-items: revert;
}

.more-from .all-posts {
  margin-left: revert;
  font-size: revert;
}

#single-post-footer {
  background-color: revert;
  padding: revert;
}

@media (min-width:992px) {
  #single-post-footer {
    padding: revert;
  }
}
#single-post-footer .card {
  background-color: revert;
  flex: revert;
  min-width: revert;
}

.previous-next-container {
  margin-top: revert;
}

.previous-next-container .previous:not(:last-child) {
  margin-bottom: revert;
}

@media (min-width:992px) {
  .previous-next-container {
    display: revert;
    margin:36px 0 0
  }
  .previous-next-container .previous.card {
    margin-bottom:0
  }
  .previous-next-container .previous.card:not(:last-child) {
    margin-right:12px
  }
  .previous-next-container .next:not(:first-child) {
    margin-left: revert;
  }
}
.reaction-links {
  text-align: revert;
  margin-bottom: revert;
}

.reaction-links .header {
  padding-bottom: revert;
}

.reaction-links .reaction-link {
  text-decoration: revert;
  font-size: revert;
}

.reaction-links .reaction-link:not(:last-child) {
  margin-right: revert;
}

.footer {
  background-color: revert;
}

#footer .footer__container {
  color: revert;
  border-top: revert;
  margin: revert;
  padding: revert;
  text-align: revert;
}

#footer .footer__container .p3:not(:last-child) {
  margin-bottom: revert;
}

@media (min-width:992px) {
  #footer .footer__container {
    display: revert;
    justify-content: revert;
    margin:0 11vw
  }
  #footer .footer__container .p3 {
    margin-bottom: revert;
  }
}
.footer--blog-page {
  background-color: revert;
}

.masonry-layout {
  display: revert;
  opacity: revert;
  transition: revert;
  margin: revert;
  padding: revert;
}

@media (min-width:992px) {
  .masonry-layout {
    display:block
  }
  .masonry-layout.masonry-layout--visible {
    opacity: revert;
    display: revert;
    flex-flow: revert;
    max-width: revert;
    margin-bottom: revert;
  }
}
.masonry-layout__column-break {
  flex-basis: revert;
  width: revert;
  list-style-type: revert;
}

.active-author {
  display: revert;
  margin-bottom: revert;
}

.active-author a:before {
  background-image: revert;
}

.active-author:last-child {
  margin-bottom: revert;
}

.active-author .active-author__bio {
  color: revert;
  font-weight: revert;
  margin-top: revert;
  display: revert;
  -webkit-box-orient: revert;
  -webkit-line-clamp: revert;
  overflow: revert;
}

.active-author .easter-egg {
  width: revert;
}

.active-author .card {
  transition: revert;
  overflow-wrap: revert;
}

.active-author .card:hover {
  box-shadow: revert;
  background-image: revert;
}

.active-author .card:hover .active-author__title {
  color: revert;
}

.active-author .card:hover .active-author__icon--featured g {
  opacity: revert;
}

.active-author .card:hover .active-author__icon--featured path {
  fill: revert;
}

@media (min-width:992px) {
  .active-author {
    width: revert;
    margin-bottom: revert;
  }
}
@media (min-width:992px) and (max-width:1311px) {
  .active-author {
    width: revert;
  }
}
.active-author__title {
  color: revert;
  display: revert;
  justify-content: revert;
  transition: revert;
  min-height: revert;
}

.active-author__word-count {
  margin-top: revert;
  display: revert;
  color: revert;
  font-weight: revert;
  height: revert;
}

.active-author__word-count svg path {
  fill: revert;
}

.active-author__icon-container {
  width: revert;
}

.active-author__icon {
  width: revert;
  height: revert;
}

.active-author__icon--word-count {
  margin-right: revert;
}

.active-author__icon--featured g {
  opacity: revert;
  transition: revert;
}

.active-author__icon--featured path {
  fill: revert;
  transition: revert;
}

.easter-egg__sign-up {
  display: revert;
  align-items: revert;
  font-weight: revert;
  color: revert;
  margin-top: revert;
}

.easter-egg__sign-up .easter-egg__icon--arrow {
  height: revert;
  width: revert;
  margin-left: revert;
}

.easter-egg__sign-up .easter-egg__icon--arrow path {
  fill: revert;
}

.active-authors__headline {
  display: revert;
  align-items: revert;
  margin: revert;
}

@media (min-width:992px) {
  .active-authors__headline {
    margin: revert;
  }
}
.active-authors__masonry-layout {
  display: revert;
}

@media (min-width:992px) {
  .active-authors__masonry-layout {
    display: revert;
  }
}
.active-authors__masonry-column:not(:last-child) {
  margin-right: revert;
}

.active-authors--mobile .button.card {
  width: revert;
}

@media (min-width:992px) {
  .active-authors--mobile {
    display: revert;
  }
}
.usage .button--start-writing {
  width: revert;
  margin-top: revert;
}

@media (min-width:992px) {
  .usage .button--start-writing {
    display: revert;
  }
}
.usage__column-layout .usage__header {
  margin-bottom: revert;
}

@media (min-width:992px) {
  .usage__column-layout {
    display: revert;
  }
}
@media (min-width:992px) {
  .usage__column {
    flex:1
  }
  .usage__column:not(:first-child) {
    margin-left:12px
  }
  .usage__column:not(:last-child) {
    margin-right: revert;
  }
}
.usage__list {
  list-style: revert;
  counter-reset: revert;
  margin: revert;
  padding: revert;
}

.usage__list li {
  counter-increment: revert;
  margin-top: revert;
}

.usage__list li:not(:last-child) {
  margin-bottom: revert;
}

.usage__list li:before {
  content: revert;
  display: revert;
  font-family: revert;
  font-size: revert;
  line-height: revert;
  height: revert;
  margin-bottom: revert;
  overflow: revert;
}

@media (min-width:992px) {
  .usage__list li {
    margin-top: revert;
  }
}
.getting-started__list {
  padding: revert;
  list-style-type: revert;
  counter-reset: revert;
}

.getting-started__list li {
  counter-increment: revert;
  margin-bottom: revert;
}

.getting-started__list li:before {
  content: revert;
  font-weight: revert;
}

.getting-started__author-code {
  margin: revert;
}

.getting-started__author-code .text-field {
  display: revert;
  width: revert;
  margin-right: revert;
}

.getting-started__author-code .button {
  width: revert;
  margin-top: revert;
}

@media (min-width:992px) {
  .getting-started__author-code {
    display: revert;
    width:100%
  }
  .getting-started__author-code .text-field {
    flex-grow: revert;
    width: revert;
    margin-right:12px
  }
  .getting-started__author-code .button {
    width: revert;
    margin-top: revert;
  }
}
.callout--warning {
  display: revert;
}

.gif-section__container {
  padding-top: revert;
}

.new-author__gif {
  margin-top: revert;
  border-radius: revert;
  border: revert;
  max-width: revert;
}

.validate-page .h1 {
  margin-bottom: revert;
}

.validate-page #captcha-form .button {
  width: revert;
  margin-top: revert;
}

@media (min-width:992px) {
  .validate-page #captcha-form .button {
    width: revert;
  }
}
:root {
  --border: revert;
  --color-default: revert;
  --color-primary: revert;
  --color-primary-opacity-8: revert;
  --color-neutral: revert;
  --color-neutral-darker: revert;
  --color-contrast: revert;
  --color-contrast-opacity-8: revert;
  --color-contrast-opacity-16: revert;
  --color-contrast-opacity-36: revert;
  --color-contrast-opacity-86: revert;
  --background-color: revert;
  --dimmed-text-color: revert;
  --dimmed-border-color: revert;
  --body-text-color: revert;
  --post-title-color: revert;
  --post-date-color: revert;
  --post-text-color: revert;
  --page-menu-link-color: revert;
  --header-author-name: revert;
  --header-listed-name: revert;
  --more-from-border-color: revert;
  --bio-color: revert;
  --wordcount-color: revert;
  --website-color: revert;
  --twitter-color: revert;
  --link-color: revert;
  --header-border-color: revert;
  --post-code-background-color: revert;
  --post-code-border-color: revert;
  --card-post-background-color: revert;
  --card-post-border: revert;
  --post-background-color: revert;
  --author-posts-background-color: revert;
  --more-posts-background-color: revert;
  --more-posts-post-background-color: revert;
  --footer-background-color: revert;
  --footer-border-top-color: revert;
  --callout-background-color: revert;
  --callout-success-border-color: revert;
  --callout-warning-border-color: revert;
  --callout-info-border-color: revert;
  --scroll-to-top-background-color: revert;
  --scroll-to-top-border: revert;
  --scroll-to-top-border-color-hover: revert;
  --author-footer-background-color: revert;
  --scroll-to-top-icon-color: revert;
  --blockquote-border-left-color: revert;
  --guestbook-border-left-color: revert;
  --author-header-info-links-separator-color: revert;
}

@media (prefers-color-scheme:dark) {
  :root {
    --border: revert;
    --color-default: revert;
    --color-primary: revert;
    --color-primary-opacity-8: revert;
    --color-neutral: revert;
    --color-neutral-darker: revert;
    --color-contrast: revert;
    --color-contrast-opacity-8: revert;
    --color-contrast-opacity-16: revert;
    --color-contrast-opacity-36: revert;
    --color-contrast-opacity-86: revert;
    --post-code-background-color: revert;
    --post-code-border-color: revert;
  }
}
@font-face {
  font-family: revert;
  src: revert;
  font-weight: revert;
  font-style: revert;
}

@font-face {
  font-family: revert;
  src: revert;
  font-weight: revert;
  font-style: revert;
}

@font-face {
  font-family: revert;
  src: revert;
  font-weight: revert;
  font-style: revert;
}

* {
  box-sizing: revert;
}

body,
html {
  margin: revert;
  font-family: revert;
  background-color: revert;
  color: revert;
  height: revert;
}

body {
  margin-left: revert;
  margin-right: revert;
}

a {
  color: revert;
  font-weight: revert;
  text-decoration: revert;
  position: revert;
}

a:before {
  content: revert;
  position: revert;
  top: revert;
  right: revert;
  bottom: revert;
  left: revert;
  background-image: revert;
  background-position: revert;
  background-repeat: revert;
  background-size: revert;
  opacity revert;
}

a:hover {
  color: revert;
}

a:hover:before {
  background-image: revert;
  opacity revert;
}

blockquote {
  border-left: revert;
  padding-left: revert;
  margin-left: revert;
}

p {
  margin: revert;
}

hr {
  display: revert;
  border: revert;
  text-align: revert;
  margin: revert;
}

hr:before {
  font-family: revert;
  font-weight: revert;
  font-size: revert;
  letter-spacing: revert;
  content: revert;
  display: revert;
  color: revert;
}

textarea {
  resize: revert;
}

.h1 {
  margin: revert;
  font-family: revert;
  font-size: revert;
  line-height: revert;
}

@media (min-width:992px) {
  .h1 {
    font-size: revert;
    line-height: revert;
  }
}
.h2 {
  margin: revert;
  font-family: revert;
  font-size: revert;
  line-height: revert;
}

@media (min-width:992px) {
  .h2 {
    font-size: revert;
    line-height: revert;
  }
}
.h3 {
  margin: revert;
  font-family: revert;
  font-size: revert;
  line-height: revert;
}

@media (min-width:992px) {
  .h3 {
    font-size: revert;
    line-height: revert;
  }
}
.h4 {
  font-size: revert;
  line-height: revert;
}

.h4,
.h5 {
  margin: revert;
  font-family: revert;
}

.h5 {
  font-size: revert;
  line-height: revert;
}

.p1 {
  margin: revert;
  font-size: revert;
  line-height: revert;
}

@media (min-width:992px) {
  .p1 {
    font-size: revert;
    line-height: revert;
  }
}
.p2 {
  font-size: revert;
  line-height: revert;
}

.p2,
.p3 {
  margin: revert;
}

.p3 {
  font-size: revert;
  line-height: revert;
}

.button {
  font-size: revert;
  line-height: revert;
  font-weight: revert;
  padding: revert;
  border-radius: revert;
  border: revert;
  color: revert;
  cursor: revert;
  text-decoration: revert;
  outline: revert;
  text-align: revert;
  background-color: revert;
  margin: revert;
  transition: revert;
}

.button svg path {
  fill: revert;
}

.button:focus {
  outline: revert;
}

.button--primary {
  color: revert;
  background-image: revert;
  background-size: revert;
  background-position: revert;
}

@media (min-width:992px) {
  .button--primary:hover {
    background-position: revert;
  }
}
.button--no-fill {
  color: revert;
  background-color: revert;
  position: revert;
}

.button--no-fill:before {
  content: revert;
  position: revert;
  top: revert;
  right: revert;
  bottom: revert;
  left: revert;
  border-radius: revert;
  background-image: revert;
  background-size: revert;
  background-position: revert;
  opacity: revert;
  transition: revert;
}

@media (min-width:992px) {
  .button--no-fill:hover {
    color:var(--color-primary)
  }
  .button--no-fill:hover:before {
    background-image: revert;
    background-size: revert;
    background-position: revert;
    background-position: revert;
    opacity: revert;
  }
}
.button--active {
  color: revert;
  position: revert;
  background-image: revert;
}

.button--active:before {
  content: revert;
  position: revert;
  top: revert;
  right: revert;
  bottom: revert;
  left: revert;
  border-radius: revert;
  background-color: revert;
  background-image: revert;
}

.button--disabled {
  background-color: revert;
  color: revert;
}

.card {
  background-color: revert;
  padding: revert;
  text-align: revert;
}

.callout,
.card {
  border-radius: revert;
  border: revert;
}

.callout {
  padding: revert;
  font-size: revert;
  line-height: revert;
  background-color: revert;
  display: revert;
}

.callout--success {
  border-left: revert;
}

.callout--warning {
  border-left: revert;
}

.callout--info {
  border-left: revert;
}

.error-message {
  color: revert;
  margin-top: revert;
}

.form-section {
  display: revert;
  flex-direction: revert;
  padding-top: revert;
}

.form-section .text-field {
  margin-top: revert;
  width: revert;
}

@media (min-width:992px) {
  .form-row {
    display: revert;
    flex-direction:row
  }
  .form-row .form-section {
    width:100%
  }
  .form-row .form-section:not(:last-child) {
    margin-right: revert;
  }
}
.headline-separator {
  height: revert;
  background-color: revert;
  flex: revert;
  margin-left: revert;
}

@media (min-width:992px) {
  .headline-separator {
    margin-left: revert;
  }
}
@media (min-width:992px) {
  .hover-container:hover .hover-content {
    display: revert;
    align-items: revert;
    justify-content: revert;
  }
}
@media (min-width:992px) {
  .hover-content {
    display: revert;
  }
}
.hover-content .hover-content__icon-container {
  width: revert;
  height: revert;
  border: revert;
  border-radius: revert;
  background-color: revert;
  display: revert;
  align-items: revert;
  justify-content: revert;
}

.hover-content .hover-content__icon {
  width: revert;
  height: revert;
}

.hover-content .hover-content__icon path {
  fill: revert;
}

.label {
  font-weight: revert;
}

.label--required:after {
  content: revert;
  color: revert;
  margin-left: revert;
}

.page-container {
  padding: revert;
}

@media (min-width:992px) {
  .page-container {
    padding: revert;
  }
}
.sublabel {
  opacity revert;
}

.text-field {
  padding: revert;
  background-color: revert;
  border-radius: revert;
  border: revert;
  color: revert;
  font-family: revert;
  font-size: revert;
  line-height: revert;
  appearance: revert;
  -webkit-appearance: revert;
}

.text-field:focus {
  outline: revert;
}

.text-field--error {
  outline: revert;
}

/* hide stuff */
#page-header,
.header-image-container,
.header-author-info .word-count__button,
.block.read-more-link,
.post-preview > .post-body.p1,
.post-date.p3,
.button.scroll-to-top__button,
.error-toast,
.reaction-links,
.more-from,
.previous-next-container,
.single-post-footer,
#footer {
  display: none;
}

/* misc */
.pages-menu__container > .pages-menu > a {
  margin-right: 1em;
}

.post-content .post-date__separator {
  margin: 0 6px;
}

.post-title.h3 {
  font-size: 1rem;
  font-weight: normal;
}

.post-title.h3 > a.post-title {
  display: list-item;
  margin-left: 1.3em;
  list-style-type: disc;
}
```

---

unfortunately i have no idea how to make the proper code block + syntax highliting work with a details tag. dumbass...
