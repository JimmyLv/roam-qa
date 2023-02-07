[[.--]]

### [Request to be featured](https://roamresearch.typeform.com/to/g5W8uCqz)

### Applying Custom Themes to you Graph by [[Conor White-Sullivan]]

{{[[video]]: https://youtu.be/UY-sAC2eGyI }}

## **Team Favorites**

### [["Advaita" aka Better Dark Age / Dracula Pro]]

Screenshots::

Dracula Pro

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamcss%2FpHrno4MPZY.png?alt=media&token=608fcfc3-3338-4f57-ab6d-c93b51c1ee9d)

Last updated:: [[December 30th, 2020]]

Designer:: [[Abhay Prasanna]]

Twitter:: [@AbhayPrasanna](https://twitter.com/AbhayPrasanna)

Love this theme? Say thanks via [PayPal](https://www.paypal.me/abhayprasanna) or Venmo @Abhay-Prasanna (all proceeds reinvested in the Roam community!)

Special Features::

Very responsive to CSS changes (update within 24 hours)

Multiple Dark Colorsets

Material Palenight

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamcss%2FTKRjaiLAWr.png?alt=media&token=d1e081e4-61ec-48a1-a7b4-5bd3152e59df)

Dark Night

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamcss%2F_XwEZNszZy.png?alt=media&token=44c6974a-ad96-4a79-870d-68563ff2f8cc)

Shades of Purple

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamcss%2FWz9h4gySQQ.png?alt=media&token=79399141-5054-4832-8971-057ee944fc8a)

Switches to Light mode based on OS setting

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamcss%2FTzMglEX3y3.png?alt=media&token=d0ffefe9-e9d9-4429-8f17-d7edae5a4dfb)

Masonry add-on

Pages stack in columns in sidebar

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamcss%2F7kcdEQWEBM.png?alt=media&token=e2f32302-310d-4619-a80d-27c48066dbd6)

Rainbow indents add-on

Colorful shadowed indent levels

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamcss%2FksQEhPdk3w.png?alt=media&token=27cc4bd1-b2c1-46ba-b757-31e50da5e957)

Code::

{{[[roam/css]]}}

```css
@import url('https://abhayprasanna.github.io/material-palenight-roam.css');
@import url('https://abhayprasanna.github.io/rainbow-indent.css');
@import url('https://abhayprasanna.github.io/dark-masonry.css') (min-width:700px);```

Replace "dark-age-dracula" with the following for other colorsets:

material-palenight-roam [*](((NfZ-xipBw)))

dark-night-roam [*](((MAx6iJEHs)))

shades-of-purple [*](((iwbzGyhHg)))

Various optional adjustments I use in my own theme (annotated in code):

{{[[roam/css]]}}

```css
@import url('https://abhayprasanna.github.io/optional.css');```

### [[Railscast]]

Screenshots::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamcss%2F866sLcv-ZR.png?alt=media&token=7656688e-3cf9-4d05-9636-16e0ec5eed96)

Last updated:: [[January 6th, 2021]]

Designer:: [[Jeff Harris]]

Twitter:: [@jeffharrissays](https://twitter.com/jeffharrissays)

Love this theme? Say thanks via [Cash App](https://cash.app/$jeffharris) or [paypal](https://paypal.me/jmharris903?locale.x=en_US)

Special Features::

Robust variables for customization

{{[[roam/css]]}}

```css

:root {
  /* Roam default variables */

  --primary-color: #137cbd;
  --s1: 8px;
  --background-color: #e1e8ed;

  /* Primary fonts */

  --main-font: 'Inter', sans-serif;
  --main-font-color: #999;
  --main-font-size: 14px;
  --code-font: 'Source Code Pro', 'Courier New', Courier, monospace;
  --code-font-color: #6d9cbe;
  --code-font-size: 0.9rem;
  --caret-color: #0080ff;

  /* Fonts */

  --alias-bg: transparent;
  --alias-font-color: #fecf2b;
  --attr-font-color: rgba(17, 137, 189, 0.65);
  --block-ref-bg: none;
  --block-ref-border: rgba(254, 207, 43, 0.6);
  --block-ref-font-size: 1em;
  --block-ref-hover: #eb9854;
  --block-ref-hover-bg: #111;
  --breadcrumb-bg: transparent;
  --breadcrumb-color: #5c7080;
  --breadcrumb-font-size: 13px;
  --breadcrumb-line-height: 0.85em;
  --calculation-color: #ff6000;
  --db-menu-bg: #333;
  --db-menu-border: #3d3d3d;
  --db-menu-header: #5c7080;
  --db-menu-item: #eb9854;
  --db-title-font-color: #eb9854;
  --db-title-hover: rgba(167, 182, 194, 0.3);
  --dialog-bg: #333;
  --dialog-font-color: #eee;
  --emphasis: #fc5963;
  --external-link-color: #8dbb40;
  --h1-font: var(--main-font);
  --h1-font-color: #1189bd;
  --h1-font-size: 2.25em;
  --h1-font__link--color: var(--page-link-color);
  --h2-font: var(--h1-font);
  --h2-font-color: #1189bd;
  --h2-font-size: 1.625em;
  --h2-font__link--color: var(--page-link-color);
  --h3-font: var(--h1-font);
  --h3-font-color: #1189bd;
  --h3-font-size: 1.2rem;
  --h3-font__link--color: var(--page-link-color);
  --hashtag: #e9892475;
  --highlight-background-color: #008aff5e;
  --highlight-font-color: #bbb;
  --highlight-link-color: #ff6000;
  --left-sidebar-font-color: #1189bd;
  --left-sidebar-font-color-hover: #e98924;
  --left-sidebar-font-size: 1rem;
  --left-sidebar-shortcuts-color: var(--left-sidebar-font-color);
  --left-sidebar-shortcuts-font-size: 1rem;
  --left-sidebar-shortcuts-title-color: var(--left-sidebar-font-color);
  --page-brackets: rgba(228, 124, 67, 0.25);
  --page-link-color: #eb9854;
  --page-link-namespace-color: #ebd454;
  --popover-font-color: #e98924;
  --popover-bg: #333;
  --ref-count-font-size: 0.8em;
  --right-sidebar-font-color: var(--main-font-color);
  --right-sidebar-link-color: #eb9854;
  --right-sidebar-bg: #323232;
  --right-sidebar-masonry-bg: var(--body-bg);
  --right-sidebar-masonry-outline: #3d3d3d;
  --right-sidebar-section-border-color: #e9892475;
  --search-bg: #252525;
  --search-body-font-color: #8a9ba8;
  --search-font-color: #af671c;
  --search-new-page-color: #8dbb40;
  --search-outline: #e9892475;
  --search-selected-row: #4c4c4c;
  --strong: #508bb5;
  --tag-font-color: #777;
  --tag-font-color-hover: #fff;
  --tag-hover-bg: #e98924;
  --tag-padding: 0.071428571em 0.428571429em 0.214285714em;
  --tag-radius: 2em;

  /* Backgrounds and objects */

  --block-highlight: #00588e;
  --block-highlight-current: rgba(255, 255, 255, 0.05);
  --block-highlight-bg: #312c28; // This is the Mentions background highlight color
  // --body-bg: #232323;
  --body-bg: #2c2c2c;
  --bullet: rgba(225, 117, 28, 0.3);
  --bullet-closed: rgba(225, 117, 28, 1);
  --bullet-closed-right-sidebar: var(--bullet-closed);
  --bullet-outline: #404040;
  --bullet-outline-highlight: #ff9500;
  --bullet-outline-hover: #ff9500b3; //recommend this be 70% of --bullet-outline-highlight
  --bullet-position: 4px;
  --bullet-version: #137cbd;
  --checkmark-border: #137cbd;
  --checkmark-bg: #555;
  --checkmark-color: #137cbd;
  --code-bg: #002b36;
  --datepicker-bg: transparent;
  --datepicker-day-wrapper: #d9822b7a;
  --datepicker-font-color: var(--popover-font-color);
  --datepicker-select-bg: #444;
  --hr: rgba(225, 117, 28, 0.5);
  --icon-bg-hover: rgba(167, 182, 194, 0.3);
  --icon-color: #e78924;
  --icon-color-hover: #e78924;
  --inline-search-bg: #333;
  --inline-comment-bg: transparent;
  --inline-comment-bg-hover: var(--reference-item-bg);
  // --left-sidebar-bg: #2b2b2b;
  --left-sidebar-bg: #323232;
  --left-sidebar-hover-bg: #1f1f1f;
  --reference-item-bg: #d8ac6e1a; // JH: Railscast uses 1 semi-transparent color for all three bg values
  --reference-item-bg-2: #d8ac6e1a;
  --reference-item-bg-3: #d8ac6e1a;
  --section-border-color: #e9892475;
  --select-bg: #232323;
  --topbar-bg: var(--body-bg);
  --topbar-border-color: #333;

  /* Misc */

  --pages-delete-bg: #222; // modal variable
  --pages-delete-border-color: #d8e1e8; // JH: modal variable, New variable TODO add to body .delete-all-dialog-items
  --pages-header-row-bg: #262626;
  --pages-header-row-font-color: #bfccd6;
  --pages-mentions-bg-empty: #3a3a3a;
  --pages-mentions-color: #ff6000;
  --pages-mentions-color-empty: #737373;
  --pages-row-highlight: #292929;
  --pages-search-bg: #3a3a3a;
  --pages-search-outline: #e9892475;
  // --pages-search-outline: var(--search-outline); //no longer exists in Roam, add if needed for Theme or replace with inherit or initial?
  --pages-table-border: #2f373d;
  --pages-sorted-color: #508bb5;

  --table-border: #444;
  --table-font-size: 0.85rem;

  --kanban-board-bg: #333333;
  --kanban-card-bg: #555555;
  --kanban-card-font-color: #6d9cbe;
  --kanban-column-bg: #454545;
  --kanban-column-font-color: #e98924;

  --encrypted-font-color: #ff6000;
  --encrypted-bg: #222;

  --pomodoro-bg: transparent;
  --pomodoro-color: #fc5963;
  --pomodoro-border: #fc596370;

  --blockquote-font-color: rgba(109, 156, 190, 0.89);
  --blockquote-font-size: 14px;
  --blockquote-border-color: #30404d;
  --blockquote-bg: none;
  --blockquote-cite: #777;

  --emoji-bg: #2d2d2d;
  --emoji-border: rgba(225, 117, 28, 0.4);
  --emoji-color: #aaa;

  --no-query-results: 'Query returned no results';
  --no-query-results-color: #fc5963;
  --query-results-border: #f2c98f1a;

  --q1: #50b2c0;
  --q2: #c5d86d;
  --q3: #ff6b6b;
  --q4: #ca7d4a;

  /* Scrollbar settings - to disable set values to none */

  --scrollbar-thumb: #323232;
  --scrollbar-track: rgba(153, 153, 153, 0.1);

  /* Saving icon colors */

  --saving-local: #99280f;
  --saving-remote: #d9822b;
  --synched: #0f9960;```

Customize query display

MINIMIZE QUERIES: add any one of the following tags before the beginning of your query (in the same block): #min-title = hides the page reference link / page title #min-con = hides the contextual reference information (breadcrumbs) #minimal = hides both the title and the context #min-q = hides the query string, similar to legacy behavior #min-all = hides everything — title, context, and query string

Expanded Bullet collapse

Fullwidth search bar

Code::

{{[[roam/css]]}}

```css
@import url('https://jmharris903.github.io/Railscast-for-Roam-Research-Theme/RailsRoam.css');```

### [[Better Roam Research]]

Screenshots::

If your OS is in Light Mode:

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FnoeJ9L0SQp.png?alt=media&token=dcfd7281-104d-4fbc-b88b-0f93de7c4f4f)

If your OS is in Dark Mode:

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FqEbHtYl5zg.png?alt=media&token=50a57675-7928-450a-b53d-23a4f5c276fc)

Designer:: [[Fabrizio Rinaldi]]

Twitter:: [@linuz90](https://twitter.com/linuz90)

Love this theme? Say thanks via [Paypal](https://www.paypal.me/linuz90)

Special Features::

#[[Dark Mode]] but only if your OS is set to dark! 

Code::

Last updated [[June 4th, 2020]]. If it's been a while, you can check [Github](https://github.com/linuz90/better-roam-research) for the latest version. 

{{[[roam/css]]}}

```css
:root {
  --font-size: 15.5px;
  --border-color: rgba(0, 0, 0, 0.08);
  --subtle-border-color: rgba(0, 0, 0, 0.05);
  --main-background-color: hsl(210, 9%, 98%);
  --body-background-color: #ffffff;
  --reference-item-background: hsl(0, 0%, 99%);
  --brackets-color: rgba(0, 0, 0, 0.25);
  --empty-text-color: hsl(203, 12%, 75%); }

.rm-title-untitled,
#block-input-ghost > span,
textarea::placeholder {
  color: var(--empty-text-color) !important; }

body,
div,
textarea,
.level2 {
  font-family: 'Quattro', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif !important; }

iframe {
  border: none !important; }

.loading-astrolabe {
  position: absolute !important;
  width: 80px !important;
  height: 80px !important;
  opacity: 0.3 !important;
  top: calc(50% - 40px) !important;
  left: calc(50% - 40px) !important; }

#roam-sidebar-logo {
  display: none !important; }

body,
#app {
  background: var(--main-background-color) !important; }

.roam-center {
  border-left: 1px solid var(--border-color) !important;
  border-top: 1px solid var(--border-color) !important;
  border-right: 1px solid var(--border-color) !important;
  border-radius: 6px;
  box-shadow: 0px 2px 14px rgba(0, 0, 0, 0.04) !important;
  overflow: visible !important;
  background: var(--body-background-color) !important;
  margin-top: 10px;
  margin-right: 16px;
  margin-left: 16px; }
  .roam-center > div:first-child {
    padding-right: calc(0.5 * (100% - 820px)) !important;
    padding-left: calc(0.5 * (100% - 820px)) !important; }

.roam-topbar {
  background: var(--main-background-color) !important; }
  .roam-topbar input#find-or-create-input {
    box-shadow: none !important;
    border: 1px solid var(--border-color) !important; }

.roam-body,
.roam-topbar,
#right-sidebar,
.roam-sidebar-container {
  background: transparent !important; }

#right-sidebar {
  border: none !important;
  transition: none !important;
  overflow: hidden !important; }
  #right-sidebar h1 {
    font-size: 18px !important; }
  #right-sidebar #roam-right-sidebar-content > div[style] {
    border-bottom: 1px solid var(--subtle-border-color) !important; }
  #right-sidebar .hoverparent,
  #right-sidebar .react-resizable {
    max-width: 100% !important; }
    #right-sidebar .hoverparent img,
    #right-sidebar .react-resizable img {
      max-width: 100% !important; }

.rm-page-ref-tag {
  color: #9099a1 !important; }

span.checkmark {
  top: -2px; }

.rm-level1 div,
.rm-level1 textarea {
  font-size: 22px !important;
  line-height: 1.5 !important; }

.rm-level2 div,
.rm-level2 textarea {
  font-size: 20px !important;
  line-height: 1.5 !important; }

.rm-level3 div,
.rm-level3 textarea {
  font-size: 18px !important;
  line-height: 1.5 !important; }

.level2 {
  font-weight: inherit !important; }

.roam-log-container .roam-log-page {
  border-top: 1px solid var(--subtle-border-color) !important; }
  .roam-log-container .roam-log-page:first-child {
    min-height: 0 !important;
    border-top: none !important; }

.rm-reference-item {
  background: var(--reference-item-background) !important;
  border: 1px solid #f0f0f0 !important;
  border-radius: 6px !important;
  padding: 8px 10px 8px 2px !important; }
  .rm-reference-item .rm-block-text {
    font-size: var(--font-size) !important; }

.CodeMirror {
  font-size: 13px !important; }

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover,
.roam-body
.roam-app
.roam-sidebar-container
.roam-sidebar-content
.starred-pages-wrapper
.starred-pages
.page:hover {
  color: inherit !important;
  background-color: transparent !important; }

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper,
.roam-body
.roam-app
.roam-sidebar-container
.roam-sidebar-content
.starred-pages-wrapper
.starred-pages
.page,
.bp3-minimal > div {
  color: #666666 !important;
  font-size: 13px !important; }

.roam-sidebar-content {
  padding: 0 !important; }
  .roam-sidebar-content > div:not(.log-button):not(:first-child) {
    padding: 0 !important; }
  .roam-sidebar-content > div:first-child {
    padding-bottom: 18px !important; }

.starred-pages-wrapper > div:first-child {
  display: none; }
.starred-pages-wrapper .flex-h-box,
.starred-pages-wrapper .flex-h-box span {
  font-size: 13px !important;
  opacity: 0.6 !important; }

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button,
.roam-body
.roam-app
.roam-sidebar-container
.roam-sidebar-content
.starred-pages-wrapper
.starred-pages
.page {
  padding: 6px 24px 6px !important; }

.bp3-icon-small {
  padding-left: 24px !important; }

.rm-block-text {
  max-width: 640px !important;
  font-size: var(--font-size) !important; }

.block-bullet-view {
  margin-bottom: 3px !important; }

.roam-article > div > div h1 {
  font-size: 26px !important;
  font-weight: 700 !important;
  height: auto !important;
  line-height: 1.5 !important; }

.rm-title-display,
.rm-title-textarea {
  height: auto !important;
  line-height: 1.5 !important; }

.roam-log-container .roam-log-preview h1 {
  font-size: 22px !important;
  font-weight: 700 !important; }

strong {
  font-weight: 700 !important; }

.block-border-left {
  border-left-color: var(--subtle-border-color) !important; }

.rm-reference-main div > strong {
  color: gray !important; }

@media (prefers-color-scheme: dark) {
  body {
    background: #171717 !important; }

  #app {
    filter: invert(1) hue-rotate(180deg) !important; }

  img,
  div#buffer,
  .bp3-portal,
  .intercom-app,
  .loading-astrolabe,
  .bp3-dialog,
  .twitter-tweet,
  iframe {
    filter: invert(1) hue-rotate(180deg) !important; }

  .roam-highlight {
    background-color: #e2cb47 !important; }

  .bp3-overlay-backdrop {
    background-color: rgba(255, 255, 255, 0.7) !important; }

  :root {
    --border-color: rgba(0, 0, 0, 0.07) !important;
    --subtle-border-color: rgba(0, 0, 0, 0.05) !important;
    --main-background-color: hsl(0, 0%, 96%) !important;
    --body-background-color: hsl(0, 0%, 90%) !important;
    --reference-item-background: hsl(0, 0%, 93%) !important;
    --brackets-color: rgba(0, 0, 0, 0.3) !important;
    --empty-text-color: hsl(203, 5%, 70%); } }```

### [[Leyendecker]]

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2Ffc9tIphX_X.png?alt=media&token=f6c09e01-742a-478d-a537-0b3a88796325)

Designer:: [[Maggie Appleton]]

Twitter:: [@mappletons](https://twitter.com/mappletons)

Love this theme? Say thanks via [Paypal](https://paypal.me/maggieappleton)

Special Features::

Queries and Kanbans got some extra love. 

Custom data-tags are all at the end of the CSS file, which you'll probably want to edit/customise. 

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FER9x_LvrLc.png?alt=media&token=4860ec31-f27e-45c7-adaa-194594cc55e2)

Code::

Last updated [[June 4th, 2020]]

[[Site-wide]]

{{[[roam/css]]}}

```css
h1,
h2,
h3,
h4,
h5,
h6 {
    font-family: "Lato", sans-serif;
    font-size: 3em;
}
div,
textarea {
    font-weight: 400;
    color: #3F4758;
    font-size: 1.002em;
}
.roam-block-container {
    max-width: 1000px;
}

.rm-pomodoro {
    background: #fff !important;
    color: #ff4747 !important;
    padding: 4px 14px;
    line-height: 2em;
    font-weight: 600;
    border-radius: 2em;
    border: 1px solid #ff474770;
}

.rm-pomodoro {
    background: #ff6956 !important;
    color: #fff !important;
    padding: 4px 14px;
    line-height: 2em;
    font-weight: 600;
    border-radius: 2em;
    border: 1px solid #ed5845;
}

.rm-pomodoro::first-letter {
  margin-right: 8px;
}

.rm-query {
    border: 0.5px solid #e4e9ec;
    border-radius: 5px;
    
}

.rm-query .rm-query-title {
    background-color: #f7f8f8;
    padding: 0.8em;
    color: #d1dbe2;
    font-size: 80%;
}

.rm-reference-main.rm-query-content {
    padding: 0.8em;
}

.rm-reference-main .rm-reference-item .rm-block-text {
    font-size: 90%;
}

.rm-ref-page-view-title span {
    
}

.rm-reference-main .rm-reference-item .controls {
    margin-left: -1em;
}

.rm-ref-page-view {
    padding: 0.4em 0.2em;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
    padding: 6px;
}

div.flex-v-box.starred-pages-wrapper > div.flex-h-box > span {
    font-size: 14px !important;
    opacity: 80%;
    letter-spacing: 0.04em;
}

div.roam-sidebar-container.noselect > div > div {
    font-size: 14px !important;
    letter-spacing: 0.03em;
    
}

#block-input {
    background: white;
}

.roam-body #block-input > span > div {
    padding: 6px 24px;
    background: white;
}

span.bp3-icon-small.bp3-icon-star {
    display: none;
    visibility: hidden;
}

.roam-block {
    max-width: 850px;
}

#right-sidebar > div {
    background-color: #f7f8fa;
    border-left: 1px solid #e9ebef;
}
.controls .simple-bullet-outer .simple-bullet-inner {
    background-color: #e5e9f2;
}
.block-border-left {
    border-left: 1px solid #f3f6f7;
}
.kanban-board {
    background-color: #fff;
}
.kanban-card {
    background-color: white;
    margin: 8px;
    box-shadow: 0px 1px 2px #9eb3c0a8;
    padding: 10px;
    border-radius: 2px;
    line-height: 1.3em;
}
.kanban-title {
    text-align: center;
    font-weight: 600;
    font-size: 1.1em;
    opacity: 80%;
    color: #485f6f;
    padding-top: 8px;
    border-bottom: 1px solid #c5d1d8;
}
.kanban-column {
    background-color: #e7eff3;
    margin: 0px 4px 0px 4px;
    padding: 4px;
    min-width: 200px;
    border-radius: 3px;
}


.rm-block-ref::before {
    content: '';
    display: inline-block;
    width: 2px;
    border-radius: 40px;
    height: 12px;
    background: #ff913c;
    margin-right: 8px;
}
.rm-block-ref {
    border-bottom: none;
    font-size: 1em;
    color: #515e70;
}
.rm-block-ref:hover {
    background: none;
    cursor: pointer;
}
.checkmark {
    background: #fff;
}
.check-container input:checked ~ .checkmark {
    background: #33bdea;
}
.check-container input:checked ~ .checkmark:after {
    border-color: #fff;
}
.rm-reference-item {
    margin-top: 8px;
    border-radius: 6px;
    border: 1px solid #e4e9ee;
    margin-right: 8px;
    flex: 1 1 100%;
    word-break: break-word;
    background-color: #f7f9fb;
    padding: 8px;
}

.rm-level2 {
    font-size: 1.5em;
}
.rm-level3 {
    color: #939aae;
    font-weight: 400;
    font-size: 1.3em;
}
.rm-page-ref {
    color: #9aabd0;
}
.rm-page-ref-link-color {
    color: #ec6f35;
    font-weight: 600;
}
a {
    color: #8A3CC8;
}
.intercom-app,
.intercom-launcher-frame,
#intercom-container {
    display: none !important;
}
.roam-body .roam-app .roam-sidebar-container {
    background-color: white;
    border-right: 1px #eee solid;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page,
.roam-body .roam-app .roam-sidebar-container > * {
    opacity: 80%;
    box-shadow: none;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
    background: white;
    color: black;
    opacity: 100%;
}
#buffer.tall {
    height: calc(100vh - 50px) !important;
}
.check-container {
    padding-right: 4px;
}
span.rm-page-ref {
    border-radius: 2px;
    padding-left: 1px;
    padding-right: 1px;
}
.content span.rm-page-ref {
    padding: 4px 1px 1px;
    /* required for fixing azo */
}
.center-proj {
    text-align: center;
}

```

[[Tag Styles]]

{{[[roam/css]]}}

```css

/* Custom data tags */
span.rm-page-ref[data-tag="Tweet"] {
    background: #81D5ED !important;
    color: white !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Literature Notes"] {
    background: #9769FF !important;
    color: white !important;
    padding: 3px 7px;
    font-weight: 500;
    line-height: 2em;
}


span.rm-page-ref[data-tag="Evergreens"] {
    background: #0DBAC6 !important;
    color: #fff !important;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Seedling"] {
    color: #0dbac6 !important;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"] {
    color: #FCB815 !important;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"]:before {
    content: '✦ '
}

span.rm-page-ref[data-tag="Illustrated Notes"] {
    color: #7172FC;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Garden Notes"] {
    color: #9DBC13;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Video Tutorial"] {
    color: #db3b8d;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Essay"] {
    background: #ADCB2A;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Livestream"] {
    color: #B979CF;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Talk"] {
    background: #7172FC;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Waiting"] {
    background: #F9C866;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Researching"] {
    background: #FF9D66 !important;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Synthesising"] {
    background: #FC766F !important;
    color: #fff !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Alive"] {
    background: #EE5F85 !important;
    color: #fff !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}```

### [[Zenith]]

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FpF2OCzwlH2.png?alt=media&token=4bd42cd5-cd10-49a6-a915-a328ff067467)

Designer:: [[Azlen Elza]]

Twitter:: [@azlenelza](https://twitter.com/azlenelza) 

Love this theme? Say thanks via [Paypal](https://www.paypal.me/azlenelza). 

Also created [[Cosmonaut]] and [[Yggdrasil]]

Special Features::

Collapsible columns -- side-by-side view for items opened in the sidebar 

Searchbar appears in main page 

Overlay side-by-side view over graph/diagram

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FOAvb9EDHlf.png?alt=media&token=c0737a55-e90a-4f85-baa3-cc4797b24834)

Code::

{{[[roam/css]]}}

```css
/* IMPORT CORE THEME */
@import url('https://azlen.github.io/roam-themes/core.css');

/* GOOGLE FONTS */
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital,wght@0,400;0,700;1,400;1,700&display=swap');	

:root {	
    --page-width: 616px;
    --page-order: row-reverse; /* new pages show up to the right */
    /*--page-order: row; /* new pages show up to the left */
    
    --header-font: "Source Sans Pro", "Inter", sans-serif;	
    --body-font: "Source Sans Pro", "Inter", sans-serif;	
    	
    --bg-color: #EEEEEE;	
    --page-color: rgba(255, 255, 255, 0.95);	
    	
    --text-color: #000000;	
    --icon-color: #5c7080;
    --bullet-color: rgba(0, 0, 0, 0.2);	
    	
    --page-shadow: 0px 8px 14px rgba(0, 0, 0, 0.05);	
    	
    --color-primary: 73, 197, 91;	
    --color-primary-contrast: #FFFFFF;	
    --color-secondary: 147, 100, 235;

    --color-secondary-contrast: #FFFFFF;	
}

/* CHANGE COLOURS IN CANVAS */
canvas[data-id="layer2-node"] {	
    filter: invert(1) hue-rotate(110deg) saturate(2.5);	
}```

## **Dark Modes**

### [[Cosmonaut]]

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FZqga3Oe0uc.png?alt=media&token=ca5c4739-ef61-4dea-a241-eaa81a5450bf)

Designer:: [[Azlen Elza]]

Twitter:: [@azlenelza](https://twitter.com/azlenelza) 

Love this theme? Say thanks via [Paypal](https://www.paypal.me/azlenelza). 

Also created [[Zenith]] and [[Yggdrasil]]

Special Features::

#[[Dark Mode]]

Variation on [[Zenith]] which has: 

Collapsible columns -- side-by-side view for items opened in the sidebar 

Searchbar appears in main page 

Overlay side-by-side view over graph/diagram

Code::

{{[[roam/css]]}}

```css
/* IMPORT CORE THEME */
@import url('https://azlen.github.io/roam-themes/core.css');

/* GOOGLE FONTS */
@import url('https://fonts.googleapis.com/css2?family=Oxanium:wght@600&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Ubuntu:ital,wght@0,400;0,700;1,400;1,700&display=swap');

/* VARIABLES */
:root {
    --page-width: 616px;
    
    --header-font: "Oxanium", "Inter", sans-serif;
    --body-font: "Ubuntu", "Inter", sans-serif;
    
    --bg-color: #000000;
    --page-color: rgba(44, 44, 44, 0.95);
    
    --text-color: #FFFFFF;
    --icon-color: rgb(102, 102, 102);
    --bullet-color: rgba(255, 255, 255, 0.3);
    
    --page-shadow: 0px 8px 14px rgba(0, 0, 0, 0.25);
    
    --color-primary: 47, 155, 249;
    --color-primary-contrast: #FFFFFF;
    --color-secondary: 228, 78, 244;
    
    --color-secondary-contrast: #FFFFFF;
}

/* CHANGE COLOURS IN CANVAS */
canvas[data-id="layer2-node"] {
    filter: invert(1) contrast(1.1) hue-rotate(180deg) saturate(2);
}

/* CODE BLOCK STYLING */
/* modified from https://codemirror.net/demo/theme.html#night */
.CodeMirror { background: var(--bg-color) !important; color: #f8f8f8 !important; }
div.CodeMirror-selected { background: #447 !important;  }
.CodeMirror-line::selection, .CodeMirror-line > span::selection, .CodeMirror-line > span > span::selection { background: rgba(68, 68, 119, .99); }
.CodeMirror-line::-moz-selection, .CodeMirror-line > span::-moz-selection, .CodeMirror-line > span > span::-moz-selection { background: rgba(68, 68, 119, .99); }
.CodeMirror-gutters { background: var(--bg-color); border-right: 1px solid #252525; }
.CodeMirror-guttermarker { color: white !important; }
.CodeMirror-guttermarker-subtle { color: #bbb !important; }
.CodeMirror-linenumber { color: #f8f8f8; }
.CodeMirror-cursor { border-left: 1px solid white !important; }
span.cm-qualifier { color: #666666 !important; }
span.cm-comment { color: #C71FF9 !important; }
span.cm-atom { color: #B58AFD !important; }
span.cm-number, span.cm-attribute { color: #ffd500 !important; }
span.cm-keyword { color: #599eff !important; }
span.cm-string { color: #37f14a !important; }
span.cm-meta { color: #369BFF !important; }
span.cm-variable-2, span.cm-tag { color: #99b2ff !important; }
span.cm-variable-3, span.cm-def, span.cm-type { color: white !important; }
span.cm-bracket { color: #8da6ce !important; }
span.cm-builtin, pan.cm-special { color: #ff9e59 !important; }
span.cm-link { color: #845dc4 !important; }
span.cm-error { color: #F41000 !important; }
.CodeMirror-activeline-background { background: #1C005A !important; }
.CodeMirror-matchingbracket { outline:1px solid grey !important; color:white !important; }```

## **Feature Expansions**

### Nested Links

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2Fqr3tGRCd-s.png?alt=media&token=31913a3e-546a-4955-87fe-2c9ad8fd160f)

Designer:: [[Cato Minor]]

Twitter:: [@CatoMinor3](https://twitter.com/CatoMinor3)

Love this theme? Say thanks via [Paypal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=6AMGMUDRX29XU&source=url)

Special Features::

Additional underlining for nested tags 

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FNRBiiUtnF-.png?alt=media&token=233612e7-2aeb-4d13-b28e-8b9cc806d173)

Code::

Last updated [[June 4th, 2020]]

{{[[roam/css]]}}

```css
:root {
    --custom-background-color: lightsteelblue;
    --custom-background-color-hover: orange;
    }


.rm-page-ref-link-color{
   color:black !important;
    background: linear-gradient(0deg, var(--custom-background-color) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
    line-height: 24px;
    padding-bottom: 4px;
}

.rm-page-ref-link-color:hover{
   color:black !important;
    background: linear-gradient(0deg, var(--custom-background-color-hover) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
    text-decoration: none;
    line-height: 24px;
    padding-bottom: 4px;
}

.rm-page-ref-link-color .rm-page-ref-link-color {
color: black !important;
  background: linear-gradient(0deg, var(--custom-background-color) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
   line-height: 28px;
    padding-bottom: 8px;
}

.rm-page-ref-link-color .rm-page-ref-link-color:hover {
color: black !important;
  background: linear-gradient(0deg, var(--custom-background-color-hover) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
   line-height: 28px;
    padding-bottom: 8px;
}


.rm-page-ref-link-color .rm-page-ref-link-color .rm-page-ref-link-color {
color: black !important;
background: linear-gradient(0deg, var(--custom-background-color) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
   line-height: 32px;
    padding-bottom: 12px;
}


.rm-page-ref-link-color .rm-page-ref-link-color .rm-page-ref-link-color:hover {
color: black !important;
background: linear-gradient(0deg, var(--custom-background-color-hover) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
   line-height: 32px;
    padding-bottom: 12px;
}```

## **More Colors**

### [[Yggdrasil]]

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FT0iQmFOXwm.png?alt=media&token=3cdca40f-d2bb-4217-9f26-b44c825f88be)

Designer:: [[Azlen Elza]]

Twitter:: [@azlenelza](https://twitter.com/azlenelza) 

Love this theme? Say thanks via [Paypal](https://www.paypal.me/azlenelza). 

Also created [[Cosmonaut]] and [[Zenith]]

Special Features:: 

Collapsible columns -- side-by-side view for items opened in the sidebar 

Searchbar appears in main page 

Overlay side-by-side view over graph/diagram

Code::

{{[[roam/css]]}}

```css
/* IMPORT CORE THEME */
@import url('https://azlen.github.io/roam-themes/core.css');

/* GOOGLE FONTS */
@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,700;1,400;1,700&display=swap');

/* VARIABLES */
:root {
    --page-width: 616px;
    
    --header-font: "Crimson Text", serif;
    --body-font: "Crimson Text", serif;
    
    --bg-color: #f5f1e2;
    --page-color: rgba(236, 231, 209, .95);
    
    --text-color: #000000;
    --icon-color: #5c7080;
    --bullet-color: rgba(0, 0, 0, 0.2);
    
    --page-shadow: 0px 8px 14px rgba(0, 0, 0, 0.02);
    --color-primary: 181, 124, 38;
    --color-primary-contrast: #FFFFFF;
    --color-secondary: 100, 181, 38;
    
    --color-secondary-contrast: #FFFFFF;
}

/* YGGDRASIL CUSTOM STYLES */

.rm-page-ref-tag {
    padding: 3px 6px 2px 6px;
}

/* reverse colours for saving / saving-remote so that green is used for "saved" */
.rm-saving-icon .rm-synced {
    background-color: rgb(var(--color-secondary));
}
.rm-saving-icon .rm-saving-remote {
    background-color: rgb(var(--color-primary));
}

.block-bullet-view .bp3-button:not([class*="bp3-icon"]) {
    padding: 5px 14px 0px 14px!important;
}

.kanban-card {
    box-shadow: 0px 1px 2px rgba(0,0,0, 0.3);
}
.kanban-column {
    background-color: var(--bg-color);
}

/* CHANGE COLOURS IN CANVAS */

canvas[data-id="layer2-node"] {
    filter: invert(1) hue-rotate(170deg) saturate(2.5);
}```

## **Block Level Customizations**

from [[Maggie Appleton]] in [[Leyendecker]]

[[Tag Styles]]

{{[[roam/css]]}}

```css

/* Custom data tags */
span.rm-page-ref[data-tag="Tweet"] {
    background: #81D5ED !important;
    color: white !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Literature Notes"] {
    background: #9769FF !important;
    color: white !important;
    padding: 3px 7px;
    font-weight: 500;
    line-height: 2em;
}


span.rm-page-ref[data-tag="Evergreens"] {
    background: #0DBAC6 !important;
    color: #fff !important;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Seedling"] {
    color: #0dbac6 !important;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"] {
    color: #FCB815 !important;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"]:before {
    content: '✦ '
}

span.rm-page-ref[data-tag="Illustrated Notes"] {
    color: #7172FC;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Garden Notes"] {
    color: #9DBC13;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Video Tutorial"] {
    color: #db3b8d;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Essay"] {
    background: #ADCB2A;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Livestream"] {
    color: #B979CF;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Talk"] {
    background: #7172FC;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Waiting"] {
    background: #F9C866;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Researching"] {
    background: #FF9D66 !important;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Synthesising"] {
    background: #FC766F !important;
    color: #fff !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Alive"] {
    background: #EE5F85 !important;
    color: #fff !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}```

