## [Updating Roam]([[Updating Roam]])

## [Change Log Archive](https://roamresearch.com/#/app/help-archive/page/dxTi-iUs2)

## **New Changes**

[[December 20th, 2022]]

Fixes a couple of performance issues, should be noticeable especially for [[Local Graph]]s

[[November 30th, 2022]]

[[Roam Extensions]]

# Roam reference expands

show the path of the block reference

![](https://github.com/dive2Pro/roam-reference-expand/raw/49e028ae09c5ec50eeec4436bd81247b7a7e0685/SCR-20221124-d9c.png)

![](https://github.com/dive2Pro/roam-reference-expand/raw/master/reference%20extends.gif)

# Uninstall

All configurations are stored on the [[roam/reference extends/config]] page and need to be removed manually if you want to uninstall the plugin cleanly.

# Mapbox

Render interactive maps directly in your graph!

## Usage

Type `{{maps}}` in a block. When the block renders, an interactive map will render in its place!

To position the map at a particular center, create a child block with text "Center". Under that block, put in the latitude and longitude coordinates of the center delimited by a comma.

To start the map at a particular zoom level, create a child block with text "Zoom". Under that block, put in the zoom level value which should be a number. A minimum value of 0 is zoomed all the way out and a maximum value of 18 is zoomed all the way in.

To add Markers to the map, create a child block with text "Markers". Under that block, add one child for every marker you want to include. In the block, write the text you'd like as the label of the block. As a child of **that** block, put the latitude and longitude coordinates of the marker.

For example, the following configuration will have to be set as the child of the block to produce the map below:

Center

32.715736, -117.161087

Zoom

12

Markers

David Vargas

32.7, -117.2

RoamJS

32.72, -117.1

If the Marker text is already a tag in your graph, clicking on the marker pin will take you to that page. Shift clicking the marker will open the tag in the sidebar.

You could also filter the markers that are displayed on your map. Clicking the wrench icon on the top right will open the settings overlay, where you could specify a tag to filter by. All markers that are pages that have a block with the entered tag will remain on the map while the rest get filtered out.

[[November 29th, 2022]]

[[Roam Extensions]]

# Oura Ring

Import your Oura Ring daily summaries on a given day into your daily note page!

## [🔗](https://github.com/dvargas92495/roamjs-oura-ring#usage)Usage

You'll first need to add your personal access token associated with your Oura Ring account to the Token field in your Roam Depot Settings. The extension needs this in order to access your personal data. [Click here](https://cloud.ouraring.com/personal-access-tokens), to generate your own personal access token.

To import your Oura Ring data to your daily note page, open the Command Palette and enter "Import Oura Ring". If the current page is a Daily note page, it will query the day before the page title, since you usually want to track last night's sleep. Otherwise, it will query yesterday's data by default. It will output the following text:

```javascript
Bedtime Start:: hh:mm:ss
Bedtime End:: hh:mm:ss
Sleep Duration:: hh:mm:ss
Total Sleep:: hh:mm:ss
Total Awake:: hh:mm:ss
Light Sleep:: hh:mm:ss
Rem Sleep:: hh:mm:ss
Deep Sleep:: hh:mm:ss
Day Start:: hh:mm:ss
Day End:: hh:mm:ss
Low Activity:: hh:mm:ss
Medium Activity:: hh:mm:ss
High Activity:: hh:mm:ss
Rest Activity:: hh:mm:ss
Readiness Score:: hh:mm:ss```

You can also import the data by creating a button by typing `{{import oura ring}}` into a page and clicking the button.

# Roam native dark theme

![](https://github.com/dive2Pro/roam-native-dark/raw/master/SCR-20221120-hek.png)[🔗](https://github.com/dive2Pro/roam-native-dark/blob/master/SCR-20221120-hek.png)

![](https://github.com/dive2Pro/roam-native-dark/raw/master/SCR-20221120-hfj.png)[🔗](https://github.com/dive2Pro/roam-native-dark/blob/master/SCR-20221120-hfj.png)

[[November 28th, 2022]]

[[Roam Extensions]]

# SamePage

Official Roam client into [SamePage](https://samepage.network/) - the intra tool-for-thought protocol.

Use SamePage to connect your Roam Graph to other notebooks to sync changes across them, perform cross notebook queries, and more! To get started, install this extension and request an invite code by emailing [support@samepage.network](mailto:support@samepage.network). Check out our docs at https://samepage.network/docs!

## WARNING

The SamePage family of extensions are still **in beta** and are not considered stable yet for real or sensitive data. All data shared on SamePage is considered public and probability of data loss is high.

Previously, extensions were not listed on the change log, please check out our [github](https://github.com/Roam-Research/roam-depot) for a [full list of new extensions and updates](https://github.com/Roam-Research/roam-depot/pulls?q=is%3Apr+is%3Aclosed). From now on, all new extensions will be listed here

[[November 11th, 2022]]

Small fixes

Fixes issue on restore graph from EDN where some graphs would get stuck near completion

Fixes "Roam was not built in a day" error that would arise sometimes when collapsing right sidebar windows corresponding to pages

[[October 6th, 2022]]

[[New Features]]

Single Block Multiselect Mode

Select blocks but not their children or select non consecutive blocks and perform bulk actions on them

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FCtabMYCHRV.png?alt=media&token=2ff14e70-6c2c-4e3b-8dc0-318966366c07)

**How to use**

Toggle the mode on / off with `ctrl-m` (PC) or `cmd-m` (Mac) (customizable)

Then click a checkbox to select it

Shift click another checkbox to select a range between that checkbox and the last one selected

**Available commands**

Drag and dropping blocks

Right click context menu

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FhmG851Z2bl.png?alt=media&token=f2366b67-bd41-4e3c-b373-46bbee59f956)

This feature is still a work in progress.

Key commands (tab, shift-tab etc) do not work with it

[[September 30th, 2022]]

Small fix: if a window already exists in the sidebar and it is tried to open again, it jumps up to the top of the sidebar

A number of changes throughout the last week for integration of write actions with the new backend API

[[Developer Notes]]: Checkout [Roam Backend API (Beta) docs](https://roamresearch.com/#/app/developer-documentation/page/W4Po8pcHQ). 

New addition: [Write actions](https://roamresearch.com/#/app/developer-documentation/page/J-hxpYKmK)

[[September 7th, 2022]]

[[New Features]]  #[[Improvements]]

[Blueprint Color](https://blueprintjs.com/docs/versions/3/#core/colors) palettes for code blocks (these colors match what is used in Roam)

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FtBmBkVpT0d.png?alt=media&token=35ab4556-dbd5-4694-9621-63a726147657)

#[[Quality of Life Improvements]] #[[Bug Fixes]]

Fixed checkbox alignment on [[Firefox]]

**Before**

![Screenshot 2022-09-07 at 17 57 57](https://user-images.githubusercontent.com/285292/188948053-ba930d81-6bc4-4de9-8d13-d0fe9acc01f5.png)

**After**

![Screenshot 2022-09-07 at 17 58 16](https://user-images.githubusercontent.com/285292/188948064-96cd01d0-6822-4294-b3fb-19462121368a.png)

[[August 18th, 2022]]

[[New Features]] __sort of__ #[[Tag Styles]]

We decided to include some of the most useful [[roam/css]] [[Tag Styles]] we've developed for ourselves, you may find helpful/inspiring .rm-E  .rm-g  and .rm-hide

## .rm-E 

Behavior::

Blocks tagged with `#.rm-E` will display their immediate children next to them, 

rather than indented below them

Use Cases::

When you want a sort of [[Mind Map]] light behavior, 

or just want to view things side by side

🤷‍♂️ it's nice to have when you want it not much more to it than that

Example::

A #.rm-E 

B

Note that this only impacts the first level of nesting

C

If you want to go further, you have to keep using the tag

D [[.rm-E]]

Using the link, not the tag

so you can see where it is used

E [[.rm-E]] 

 since this class hides itself when used as a tag

## .rm-g 

Behavior::

Blocks tagged with `#.rm-g` are hidden when they are open  - revealing the children nested within them 

Children are styled to look like they are one level higher in the block hiearchy than they are -- useful for adding meta-data tags without visually cluttering your outline.

Use Cases::

when you want to group a collection of items and hide the block that contains them

Example::

[[.rm-g]] #[[Fruits]] 

Apples

Pears

Cherries

## .rm-hide

Use Cases::

When you want to add some info to a block without visually cluttering things up - but still allow the info to be discoverable easily

Behavior::

This block only displays when it is open - when it is closed, it is replaced with a very light bar across it's length

The bar get's darker on hover, and which

when you click it - it opens the block

In some ways a mirror of .rm-g  

Example::

{{[[DONE]]}} This is a task that I'm hiding the metadata for

Total Time:: 2 min #.rm-hide  

Start time:: 17:26

End time:: 17:28  

The block above me ((((jq0MYtn5U)))) has a hidden child - hover between us and click the bar to expand it - or arrow key up from me, or down from it, and you'll see it

Have some hidden children here too

#.rm-hide 

hidden children

Look between us!

[[CSS Changes]]

Zooming out from sidebar, embed-path, or backlinks now outlines the block you were originally focused on, rather than coloring the block and all it's children with an obnoxious yellow

Example::

Shift click on this reference [[>]] Socrates is Mortal and then click a breadcrumb in the sidebar and 

you'll see this  ->  ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FKfjpSlNswz.png?alt=media&token=7ab3240d-5f22-4292-b0d0-6ca3d217b115)

Images now display inline (previously the forced a line break)

References of blockquotes and Images now display inline

Now it is easier to use them for building up compound statements

Example::

[[>]] All Men are Mortal

[[>]] Socrates is a Man

[[>]] Socrates is Mortal

> [[IF]] [[>]] All Men are Mortal [[AND]] [[>]] Socrates is a Man 
[[THEN]] [[>]] Socrates is Mortal

[[August 17th, 2022]]

[[New Features]]  #[[Improvements]]

[[Latex]] now will parse block references, including other latex so you can comp

Example::

$$\Large$$\frac{$$n_1$$}{$$n^n$$}$$ + \sum_{i=1}^z $$\mapsto $$n^n$$$$ $$

### Recursive Latex

$$\frac{$$n_1$$}{$$n^n$$}$$

$$n_1$$

$$n^n$$

### Plain Text

\sum_{i=1}^z

^z

i=1

### Reference of Reference - to describe how variable used in another context

$$\mapsto $$n^n$$$$

Here you can describe the meaning of mapsto n^n

$$n^n$$

Here you could describe the meaning of the n^n that is being described here

### Sizing

\Large

Try changing \Large to 

\Huge

\Small

Use Cases::

Being able to separately describe each element of the equation.

#[[Quality of Life Improvements]] #[[Bug Fixes]] **[[Feature Behavior Change]]**

Behavior of [[Inline Calculator]] `{{calc: }}` for parsing block references has changed 

[[Old State]]

Previously, when you composed calculations across many blocks - all of the math text was pulled up and flattened - which could lead to unexpected behavior when building up statements and making calculations that depended on other calculations 

Example::

Wait? 2 times 4 doesn't equal 5! ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FeoLoaSY0y_.png?alt=media&token=0fb80ad2-894a-40b5-ba87-841b7fa3cd63)

After Change:: 2 times 4 = 8  ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FC500DSjbn0.png?alt=media&token=5ea62b8f-f710-4e59-ba20-b7d4e25c474e)

The old hack to get around required you to wrap block references in a `( )` to make sure that that each component in the calculation was evaluated independently before the values were aggregated  After this update, every reference used in a calculation will be wrapped in a `()` automatically before calculation is applied remember [[PEMDAS]]?

This is what is actually being evaluated now - if you're using lots of nested refs  ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2F_0bfRasZfz.png?alt=media&token=edd56c7d-6590-44be-92e3-4b187a50fad2)

[[New State]]

After this update, every reference used in a calculation will be wrapped in a `()` automatically before calculation is applied

Example::

2 times 4 = 8  ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FC500DSjbn0.png?alt=media&token=5ea62b8f-f710-4e59-ba20-b7d4e25c474e)

[Try it here](((YdPt3ZIEV)))

2 times 20 = 40, not 21

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamteam%2FZCxS2W-TvQ.png?alt=media&token=64cd1702-a33f-4517-b198-ebad16f9836c)

New Features::

Clicking the green text of the [[calc]] function has always displayed content of the internals of the calcuation, but now if you click on the = sign after doing this, you can see the fully expanded function which is being evaluated, so you can confirm that everything is happening the way you want it to 

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FvIZpt-B0OI.png?alt=media&token=a87650f5-0fcc-46c0-a31a-2231b01f9d6d)

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2F0QAGtWb2NP.png?alt=media&token=f7821d1a-5834-45bc-99c0-6240757cffcd)

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2F_0bfRasZfz.png?alt=media&token=edd56c7d-6590-44be-92e3-4b187a50fad2)

## Try it yourself

[[Z]] {{[[calc]]: ((9VZ6lwlfx)) * ((zqspvHH4e))}}

[[X]] {{calc: ((pJOOIdwKC)) + ((U35nxx0ha))}}

1

1

[[Y]] {{calc: ((xdm0aDOmu)) + ((k9UaJrwOM))}}

2

2

[[August 15th, 2022]]

[[New Features]] #[[Alpha]]

`{{embed-path: ((block-ref))}}` - Experimental new view of block embeds where path is visible and clickable - similar to what you'd see for the block in inline-references 

[[Problem it Solves]]

Often when viewing embeds, it is frustrating to not be able to see the context of the embed - the embed-path component lets you see the parent path of the block at a glance, and navigate to it quickly.

#[[CSS Changes]]

Changed the styling when you zoom out of a block in a context - like sidebar and moved the color into a css variable 

`var(--inline-highlight-color)` for the color of ^^highlights^^

`var(--highlight-color)` for color of highlighted blocks due to zooming out in a embedded context like within backlinks, sidebar, or block refs.

[[August 11th, 2022]]

[[Quality of Life Improvements]]

Search field to help you find the graph you want to switch to d

 in sidebar 

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FXqRHzdD9g9.png?alt=media&token=307c2373-aee6-4cc4-8321-8926a2aa7faa)

on all-graphs page

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FZldEt56a8N.png?alt=media&token=9f6292f0-3ec2-4117-8359-dae3760063ab)

Update to the help database to remove custom styling

 [[July 25th, 2022]]

[[RoamDepot]] #[[Plugins]]

[[PhonetoNote]]

Create a dedicated phone number to send and forward messages to a Roam graph + more

https://twitter.com/phonetonote/status/1551764556707397633?s=20&t=qEEBfrUN4jkSq9qSt5HDAQ

 [[July 19th, 2022]]

[[RoamDepot]] #[[Plugins]] 

 [[Matter]] 

 great way to sync highlights

https://twitter.com/matter/status/1549490849595080704?s=20&t=qEEBfrUN4jkSq9qSt5HDAQ

[[July 15th, 2022]]

#[[New Features]] [[RoamDepot]] #[[Major Launch]]

https://twitter.com/RoamResearch/status/1547823281478066177?s=20&t=qEEBfrUN4jkSq9qSt5HDAQ

[[RoamDepot]] #Plugins 

[[Bionic Text]]

https://twitter.com/fbgallet/status/1548083399977340930?s=20&t=qEEBfrUN4jkSq9qSt5HDAQ

[[July 11th, 2022]]

Fixed backspace deleting selected blocks when opening up the command pallete

Also added refocusing of the selected block when hitting `escape` to exit the command pallete

Increase markdown import limit from 10 to 10,000

[[June 24th, 2022]]

[[mobile]]

[[iOS]]

Fixed tab, shift-tab, backspace, and arrow keys on ipad with an external keyboard

Fixed sign in flash on app restart

Fixed saving the last used graph across app restarts

[[android]]

Fixed back gesture

Added native Google and Apple sign in

Added sign out

[[June 15th, 2022]]

[[mobile]] [[iOS]]

Apple sign in

Native google sign in

Fixed sharing text with newlines in it

Password Manager autofill for login/password

[[June 12th, 2022]]

[[Desktop App]] Links

Requires [updating](((8Dqpa2XQ5))) the desktop app to `0.0.15`

Deep links that allow one to directly navigate to a graph/page/block in the desktop app

Demo video (showing some convenient usage tricks too)

{{[[video]]: https://www.loom.com/share/fb5095868df041a597712b7403c87ed4}}

URL Format

Similar format to normal Roam web links

instead of `https://roamresearch.com/` we have `roam://`

Example

Roam web link: `https://roamresearch.com/#/app/help/page/hyL5OPFah`

Desktop app link: `roam://#/app/help/page/hyL5OPFah`

[[June 6th, 2022]]

Sign in with Apple

Report this page for public graphs

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2F_F1M_ESBjE.png?alt=media&token=3b062277-b461-4c1d-877e-260f53017f5c)

[[June 3rd, 2022]]

Fixed bug with namespaces not showing correctly

introduced yesterday in Fixed bug with changing the code block language

[[June 2nd, 2022]]

Fixed bug with changing the code block language

introduced by [parsing change](((nQ4TnZxud)))

Keep original block first in ordering of inline refs

Password reset emails now use app.roamresearch.com

[[May 25th, 2022]]

Fix the parsing of bold in italics and italics in bold (and highlight and strikethrough). It no longer matters what order you put them in.

Examples::

`**__^^bih^^__**`: **__^^bih^^__**

`__**^^ibh^^**__`: __**^^ibh^^**__

`**^^__bhi__^^**`: **^^__bhi__^^**

`__**^^ibh^^**__`: __**^^ibh^^**__

`^^**__hbi__**^^`: ^^**__hbi__**^^

`**__^^bih^^__**`: **__^^bih^^__**

Small improvement to all pages search ((Longer debounce time and normalize the search value))

[[May 23rd, 2022]]

Fix [[mobile]] quick capture crashing when displaying old quick captures

[[May 9th, 2022]]

Fixed [[mobile]] quick capture page auto complete results

[[April 4th, 2022]]

Added the ability to remove email-password login if you are also signed in with Google

[[April 3rd, 2022]]

# **Mobile App**

The Roam mobile app is now available for download on the [iOS](https://apps.apple.com/us/app/roam-mobile/id1609277273) (iphone and ipad) and [android](https://play.google.com/store/apps/details?id=com.roamresearch.relemma&hl=en_US&gl=US) app stores

[[March 10th, 2022]]

Performance improvement to opening pages with a large amount of mentions while the mentions are closed (~4x faster for a page with 6.1k mentions)

Note that this does not improve the performance of actually opening the mentions

[[March 8th, 2022]]

[[Code Block]]

[[Solidiity]] syntax highlighting support

Fixed issue with color picker showing on the `constructor` keyword

[[March 3rd, 2022]]

Fixes "All Pages" view so that all columns (Word Count, Mentions, Updated, etc) can be seen when searched

(was a CSS bug introduced some time ago)

[[February 16th, 2022]]

Apple Silicon (M1) [[Desktop App]]

Do you need to install the new App?

First [check if you are using a new M1 Mac](https://www.howtogeek.com/706226/how-to-check-if-your-mac-is-using-an-intel-or-apple-silicon-processor/)

If you are using an M1 Mac, then you should install the new app

It will be much faster than the old one

See [our migration guide](((luVUlB7o8))) for how to migrate from our old (intel) desktop app to the new (Apple Silicon) one

[[February 12th, 2022]]

Initial load memory and performance updates, related to Preparation work for graph load / memory improvements (stay tuned)

You may experience a longer load time on while your graph upgrades, you should see a message like this

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FlgY6E66Azc.png?alt=media&token=99a2a6c2-1fd2-4dc5-a6a9-53a1bc45fb53)

[[Technical Details]]

Loading from Roam's servers

up to 50% faster

up to 66% less peak memory usage (during load)

up to 20% reduction in idle memory usage (after app loads)

Loading from Indexeddb (local)

up to 16% faster

up to 40% less peak memory usage (during load)

up to 20% reduction in idle memory usage (after app loads)

up to 33% reduction in used disk space

https://www.loom.com/share/824de8dbd66c40e591eac1404e66198e

[[February 11th, 2022]]

Fix having to double click to edit text on [[iOS]] [[Safari]]

Before

{{[[video]]: https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FMgQBi2FROY.MP4?alt=media&token=10254893-b682-4a78-94e5-3ec85d632f1a}}

After

{{[[video]]: https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FXbMOzNrxpu.MP4?alt=media&token=42386235-418c-42a3-9b4c-5e6699a5cf0e}}

[[February 9th, 2022]]

Fixed bug selecting multiple blocks in embeds and linked references

[[February 7th, 2022]]

Update datascript to `1.3.9` [*](((IZesStqQa))) [*](((wBT317GzU)))

Includes [performance improvements](https://github.com/tonsky/datascript/blob/master/CHANGELOG.md#130) that might make extensions faster

Bug fixes related to Preparation work for graph load / memory improvements (stay tuned)

Delayed full release of load performance improvements

Fixed potential memory leak

Bug fixes to our update / upgrade mechanism

[[February 3rd, 2022]]

Prevent clicking out of [[Import]] while files are importing

Also added text showing progress, similar to EDN restore

Change [[Encrypted Graphs]] password

In the settings panel

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FJ6QeY8K-Zf.png?alt=media&token=2eb6670a-49b7-4696-b35d-0a2d06357815)

Fix paste bug causing images to be pasted instead of text from Microsoft Word

Revert Update datascript to `1.3.8`

Unfortunately had a bug that broke some extensions, will re release as soon as the bug is fixed

[[February 1st, 2022]]

Add icon to encrypted graphs in all graphs view

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FnyXbh-I1p-.png?alt=media&token=28305988-ec3d-40df-a6fb-68da45ee5609)

Update datascript to `1.3.8`

Includes [performance improvements](https://github.com/tonsky/datascript/blob/master/CHANGELOG.md#130) that might make extensions faster

Fix bug with [[Restore]] graph, causing some data to not be imported correctly

Fix not [[Export]]ing `:log/id`, causing daily note pages to not show up in the log

[[January 29th, 2022]]

[[Encrypted Graphs]]

Unlimited graphs for all

Increase upload file size from 100MB to 500MB

[[January 28th, 2022]]

Preparation work for graph load / memory improvements (stay tuned)

Small additions to the roamAlphaAPI (see docs [here](https://roamresearch.com/#/app/developer-documentation/page/tIaOPdXCj) for detailed changelog)

[[January 25th, 2022]]

[[Import]]

Small speed / memory improvements

Bug fix causing import to fail when importing a large amount of files

[[January 3rd, 2022]]

A major change and some minor additions to `roamAlphaAPI`, the API that roam extensions are built on top of.

If you're a dev or are interested, more details [here](https://roamresearch.com/#/app/developer-documentation/page/tIaOPdXCj)

[[December 7th, 2021]]

[[Quality of Life Improvements]]

Better error checking for queries

fixed bug where queries could previously lead to "Roam was not built in a day" errors 

[[Performance Improvements]] for imports and queries

[[November 26th, 2021]]

[[Quality of Life Improvements]]

Fix upload issues in iOS 

Automatic handling of snapshot issues

[[November 17th, 2021]]

Natural Language Date suggestions now work in "Find or Create Page" search bar

 Example screenshot

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FM37NPNdNsm.png?alt=media&token=90e32ba6-8c10-4cca-8ddc-ff78d605c8b0)

[[November 10th, 2021]]

Natural Language Dates

You can now write dates in natural language in Roam.

Write the date in square brackets [[ ]] in any format, and Roam will convert it to a date.  

Select the suggested date for it to be entered in your block. 

**Example Screenshot**

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FVzRPrXeIeH.png?alt=media&token=2173eb04-fd27-43e0-b1ca-cce79de3efde)

Some other examples you might want to try

`[[5 days ago]]`

`[[2 weeks from now]]`

`[[last friday]]`

`[[wed]]`

`[[2021-11-13]]`

`[[11-13-2021]]`

`[[17 nov 2019]]`

[[November 9th, 2021]]

[[Code Block]] [[Quality of Life Improvements]]

Updated to `codemirror.next`

Performance for large code blocks should be significantly better

Styling changes

**before**

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2Fzf8iKJxhjd.png?alt=media&token=840a48fc-71ce-4252-a6c7-d98ad3d85d3f)

**after**

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FVbqMOAbS_G.png?alt=media&token=0b5230ad-1701-4728-bf97-19d6fe45ee04)



Added `latex` and `dart` languages

Added collapsable code gutters

Added highlighting matching brackets

Changed the default font to [fira code](https://github.com/tonsky/FiraCode)

Added line wrapping

[[Example]]

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2F7wwZFV60hs.png?alt=media&token=5c951c49-c9b4-4385-b2ac-30663b6d4b32)

[[November 5th, 2021]]

[[Bug Fixes]] - fix errant text insertion for [[Firefox]] tab change

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FBBUiFSsRHb.png?alt=media&token=1a30076d-4afd-441e-9fea-311bbcfce4bb)

[[October 12th, 2021]]

Major [[Performance Improvements]] to filters on pages and backlinks 

Should be particularly noticeable on huge collections - like TODO pages or user display name pages in multiplayer graphs.

[[October 7th, 2021]]

[[Quality of Life Improvements]]

Fix [[autocomplete]] appearing offscreen in [[embed]]s, the [[Right Sidebar]] and [[mobile]]

[[embed]]

**before**

Autocomplete gets "trapped" inside of the embed

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2Fl-yBff_stw.png?alt=media&token=72683948-7ebc-440c-8bd6-0e34aff4a8bd)

and scrolls the embed, which sometimes leads to the embed getting stuck

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FVobJ470b9-.png?alt=media&token=1d4a2e9a-9b1e-401f-8182-12b962a5bfb0)

**after**

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamteam%2FdfjnNdt-Xv.png?alt=media&token=6a134550-fb43-4035-bfb3-fa5fdc74f840)

[[Right Sidebar]]

**before**

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2F0jSiiGlMdB.png?alt=media&token=b1a96c21-c829-411c-b49b-bc3d51833fa7)

also sometimes led to a similar issue [as with embeds](((d8g2z652a))), where the sidebar got stuck offscreen

**after**

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FI8GsnHl0hB.png?alt=media&token=c7a6d654-5135-4168-8f4f-c88d6ae9993f)

[[mobile]]

**before**

Autocomplete causes the whole screen to scroll to the right

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2Fj5Gk-J5ayh.png?alt=media&token=e6246ae0-ebdc-4fe2-9283-522f0f22be1e)

**after**

Autocomplete adjusts to fit the size of the screen

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FPBNQMc-v1S.png?alt=media&token=c977b686-2179-4627-8324-55867e264010)

[[September 28th, 2021]]

### [[Quality of Life Improvements]] ✨

All settings, including keyboard shortcut customizations accessible from [[Command Palette]] 

`cmd-p` on [[Mac]]

`control-p` on [[Windows]] or [[Linux]]

__handy way to discover or remember different keyboard shortcuts__

Example::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FBykG_v_8KV.png?alt=media&token=76c76dce-6346-4b6e-9435-843f07219956)

[[September 27th, 2021]]

### [[Quality of Life Improvements]] ✨

Added a shortcut (`Cmd/Ctrl+Opt+R`) to toggle [[Youtube]] [[Videos]] playback while typing in a block

Made [[Video Timestamps]] look a little nicer

### [[Bug Fixes]]  🛠

Fixed bug that caused Roam to crash when [[Query]] using `between` contained only one date

[[September 21st, 2021]]

[[Customization]] #[[End User Programming]] #[[Quality of Life Improvements]]

Custom components in [[JSX]] and [[Javascript]]

{{[[video]]: https://grain.co/highlight/NkzVPjnoX3P8gavWAVq9g00DiABYGCE1gWZIU63J}}

[[Example]]

{{[[video]]: https://grain.co/highlight/2xiEAKKj5It1deDSFzbwWMbm3JXLwqt0OdtzmQ53}}

[[September 18th, 2021]]

[[Customization]] [[Improvements]]

Styling changes applied to blocks via `#.style-tags-like-this` now propogate to references of those blocks red #.bg-red-500  #.text-white , white and blue #.bg-blue-500 #.text-white 

white

blue #.bg-blue-500 #.text-white 

red #.bg-red-500  #.text-white 

Propogates many levels up too -- see ((((q_CXURfgB)))) 

[[August 26th, 2021]]

### [[Bug Fixes]]  🛠

Fixed bug where when opening references of a block in the sidebar, two instances would show up

Fixed issues around Display Name not showing

### [[Developer Notes]] 🧑‍💻 

Fixed bug for removing window via front-end API

Fixed bug for opening mentions in sidebar via front-end API

[[August 11th, 2021]]

### [[New Features]] 🚀

You can now use [[Video Timestamps]] for Youtube videos!

Either type `/video timestamp` or hit `Cmd/Ctrl+Alt+t` under a video to enter a timestamp

Example::

{{[[video]]: https://www.youtube.com/watch?v=4yXK9OMc2OU}}

{{[[video-timestamp]]: 00:07:07}} 

#Notes Cmd+U opens search bar 

{{[[video-timestamp]]: 00:07:08}}

{{[[video-timestamp]]: 00:07:08}}

{{[[video-timestamp]]: 00:08:57}}

{{[[video-timestamp]]: 00:09:02}}

{{[[video-timestamp]]: 00:09:43}}

{{[[video-timestamp]]: 00:09:45}}

### [[Quality of Life Improvements]] ✨

Fixed [[Mobile Menu Bar]] to insert double brackets instead of single brackets

[[August 3rd, 2021]]

### [[Bug Fixes]]  🛠

Fixed bug with image links containing `\r`

[[July 11th, 2021]]

### [[New Features]] 🚀

You can now change your sign in email inside the new `Account` panel in the `Settings` menu

[[July 8th, 2021]]

### [[Bug Fixes]] 🛠 

Fixed bug where cursor remained did not move to the end of the generated template content

Fixed bug where inline css would get loaded before styling from `roam/css`

Minor bug fixes and improvements.

### [[Developer Notes]] 🧑‍💻 

`data.block.create` and `data.block.update` can now be used to set alignment,  heading, and the children blocks' view type. See [developer docs](https://roamresearch.com/#/app/developer-documentation/page/CAtB5a7wv) for more info.

[[June 23rd, 2021]]

### [[Quality of Life Improvements]] ✨

Slash menu () will only trigger when the slash is at the very beginning of a block, or preceded by a space - __not__ in the middle of a word

[[June 11th, 2021]]

### [[New Features]] 🚀

Desktop app for macOS, Linux, and Windows is out now!

Download from the `...` menu in the top right of your screen, the [[Graphs and Settings]] page, or [our home page](https://roamresearch.com)

[[June 9th, 2021]]

### [[Quality of Life Improvements]] ✨

Much faster load times when opening a graph

[[June 8th, 2021]]

### [[Bug Fixes]] 🛠 

Fixed some bugs around auto-backups, graph deletion, file manager

[[June 4th, 2021]]

### [[Quality of Life Improvements]] ✨

[[Date picker]]

Made it much faster

You can now change first day of week and see the week number

Go to `Settings > User Settings > International` to toggle.

Improved styling

{{[[table]]}}

Before

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FsfZWPjD0QC.png?alt=media&token=553e5c25-9bb5-43c1-8a1e-b2081810cce3)

After

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FQTG7J8YQV-.png?alt=media&token=d637b2c6-157f-4d2d-a810-cf0c9e1fb5f7)



[[June 2nd, 2021]]

### [[Quality of Life Improvements]] ✨

You can now copy a [[Block References]] while editing it (via `Cmd/Ctrl+Shift+C`)

You can now see other references inline for [[Block References]]. Go to `Settings > User Settings > Inline Reference Counts` to activate.

### [[Bug Fixes]] 🛠 

Fixed plaintext paste in [[Safari]]

[[May 25th, 2021]]

### [[Bug Fixes]] 🛠 

Reverted Block embeds will now be expanded by default

Comment button will no longer keep showing up after taking screenshots or switching apps

Made date picker faster

Fixed pasting multiple blocks multiple times

### [[New Features]] 🚀 #.h

Added support for [[Kroki]] diagrams ([Link](https://kroki.io)) #.h

How it works::

1. Write your kroki code in a code/regular block, for instance,
```plain text
graph TD
  A[ Anyone ] -->|Can help | B( Go to github.com/yuzutech/kroki )
  B --> C{ How to contribute? }
  C --> D[ Reporting bugs ]
  C --> E[ Sharing ideas ]
  C --> F[ Advocating ]```

2. Then use the following syntax

`{{[[kroki]]: TYPE_HERE: BLOCK_REF_HERE}}`

so for instance, `{{[[kroki]]: mermaid:((13fZ8yxDr))}}` will produce:

{{[[kroki]]: mermaid:((13fZ8yxDr))}}

Screenshots::

![](https://camo.githubusercontent.com/a4f4453e86abb6804f9f92ca477e8be856653aad9571ad62b728b22ee4e0634a/68747470733a2f2f666972656261736573746f726167652e676f6f676c65617069732e636f6d2f76302f622f666972657363726970742d35373761322e61707073706f742e636f6d2f6f2f696d6773253246617070253246726f616d2d7465616d253246682d65424e786637314a2e706e673f616c743d6d6564696126746f6b656e3d31386662333735362d336163372d346262362d616363612d393166333562626638633432)

[[May 17th, 2021]]

### [[New Features]] 🚀

You can now quickly jump to/between [[Daily Notes]] pages using the date picker!

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2Fy0yYV8dNw_.png?alt=media&token=df5b78f9-3a25-4a8c-8b7c-3eed0dba191e)

Open graph-view for page has been moved into the dropdown menu

[[Secret Feature]] - to be announced after round on testing

[[May 16th, 2021]]

### [[Quality of Life Improvements]] ✨

[[Pages]] [[Sharing]] has been re-introduced

[[Query]] will load 50 results at a time ((to prevent humongous queries from freezing Roam))

[[Query]] results can now be grouped by pages

You can now show/hide paths of blocks in [[Query]] results

### [[Developer Notes]] 🧑‍💻 

Added `data-uid` to [[Block References]]

[[May 12th, 2021]]

### [[Bug Fixes]] 🛠 

Long-pressing the expand/collapse button will expand all blocks in linked references, like in normal blocks.

Fixed PDFs not rendering

[[May 7th, 2021]]

### [[Quality of Life Improvements]] ✨

Block embeds will now be expanded by default

[[May 4th, 2021]]

### [[Quality of Life Improvements]] ✨

You can now shift-click breadcrumbs/path of zoomed-in block to open in [[Right Sidebar]]

### [[Bug Fixes]] 🛠 

Made [[Query]] and [[Linked References]] slightly faster

Pasting blocks containing images will no longer destroy block structure

Made text highlights legible in [[Block References]] previews

### [[Developer Notes]] 🧑‍💻

iFrame Components are a new possibility for extending Roam. Write components using any JS framework, host it on your own server, but interact with Roam graph data. Documentation https://roamresearch.com/#/app/developer-documentation/page/YNgZSgVSS.

[[May 3rd, 2021]]

### [[New Features]] 🚀

Hidden feature for [[Roam Team]]'s internal use, will be notifying believers if no bugs in next few days, and rest of the community shortly after that.

[[April 30th, 2021]]

### [[Quality of Life Improvements]] ✨

Added syntax highlighting for [[SPARQL]] and [[Turtle]] #[[.Kifah]]

### [[Developer Notes]] 🧑‍💻

As part of our ongoing effort to keep Roam secure, we're improving how extension settings are stored. **Please review your roam/js, roam/css and Custom Components settings and re-enable the ones you want to use again. **

### [[Bug Fixes]] 🛠

Auto-backups will no longer trigger when you switch/reload your graph.

The block info pop-up will no longer show up while dragging blocks on [[Safari]]

Fixed a bug with graph settings not appearing on local graphs

[[April 29th, 2021]]

### [[New Features]] 🚀

You can now easily manage/delete all your uploaded files by going to `... > Settings > Files`

### [[Bug Fixes]] 🛠

Pasted HTML links/images whose URL contains brackets will no longer break [[Alias]]. Go ahead, paste that [[Wikipedia]] page!

Prevent creating orphaned blocks on backspace

### [[Developer Notes]] 🧑‍💻

Moved `data-edit-time`, `data-create-time`, and `data-edit-display-name` from `span.rm-bullet` to `div.rm-block`

Added `data-edit-photo-url`

So now we can style the entire block easily based on who wrote it and access the users' profile photo url if they have one from signing in with google ((and in the future all users when we allow custom profile pictures))

[[April 28th, 2021]]

### [[Bug Fixes]] 🛠

Fixed bug which created orphan blocks when deleting in [[Linked References]]

[[April 23rd, 2021]]

### [[Bug Fixes]] 🛠

Contents of [[Kanban]] will now load normally when its children are collapsed

Pressing Enter will split the Kanban card instead of inserting an empty card

Cards can be deleted or joined like in normal blocks

Some components like images will no longer overflow the kanban

Disabled vertical scrolling on the [[Mobile Menu Bar]]

Minor performance improvements

[[April 22nd, 2021]]

### [[Bug Fixes]] 🛠

Fixed performance regression

Made settings modal mobile-friendly.

[[April 21st, 2021]]

### [[Quality of Life Improvements]] ✨

Added buttons for undo, redo, square+round brackets to the mobile menu bar!

### [[Bug Fixes]] 🛠 

Cursor will be placed correctly when adding TODO via the mobile menu bar

Multibar lines will no longer show over the mobile menu bar

[[April 20th, 2021]]

### [[Bug Fixes]] 🛠 

Fixed Graph Settings not opening and removed sharing tab for [[Local Graph]]

[[April 18th, 2021]]

### [[Quality of Life Improvements]] ✨

Improved dropdown menu 

Moved Sharing settings into its own tab

### [[Bug Fixes]] 🛠 

Redo will now work more than once

[[April 16th, 2021]]

### [[New Features]] 🚀 

Custom shortcuts! You can find them in `Settings > Hotkeys`

### [[Quality of Life Improvements]] ✨

You can now hide code blocks in search results. To toggle, go to `Settings > User Settings`.

User Settings and Graph Settings have been unified into the new Settings modal.

### [[Bug Fixes]] 🛠 

Empty `<a>` (link) tags in pasted content will no longer be rendered.

[[April 15th, 2021]]

### [[New Features]] 🚀

Unlimited [local graphs]([[Local Graph]]) are now available for all Roam subscribers!

[[April 14th, 2021]]

### [[Quality of Life Improvements]] ✨

Hitting tab while writing a page reference will autocomplete the first option

### [[Bug Fixes]] 🛠

Fixed an embed styling issue

[[April 12th, 2021]]

### [[Quality of Life Improvements]] ✨

Added [[Elixir]] as a code block option

[[April 9th, 2021]]

### [[Quality of Life Improvements]]

Page width is now persisted

[[April 7th, 2021]]

### [[Quality of Life Improvements]] ✨

Improved mobile menu bar and replaced Drawing helper button with [[TODO]] button

{{[[kanban]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2F6Xk2JBlhBF.png?alt=media&token=4da2b9c2-37de-405d-98a9-212b0f5cdffe)

After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2F6Yjwj-4gvL.png?alt=media&token=ff977aec-d135-4caa-9f76-3edf05a9b570)

**UI Updates**

Cleaned up the [[Left Sidebar]]

{{[[table]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FArTNrMYLgt.png?alt=media&token=c0a5d24c-b242-410c-a1a9-029a7638ac88)

After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FCMTzJVwz0x.png?alt=media&token=fc77ed41-c550-4859-a13b-791d0962132b)

Cleaned up [[Quick Capture]]

{{[[kanban]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FiY8WCjeeTO.png?alt=media&token=b2da9700-7c0b-42f6-8b07-4e3dd4e20f41)

After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2Feuu53BSFc4.png?alt=media&token=14a8ee81-8ea0-4439-ac74-2129804b2917)

Revamped Import modal

{{[[table]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FSX7k6To7rD.png?alt=media&token=4056c63d-e4ba-4bec-a978-dfcefac1dcc9)


After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FkXpJm3dgXf.png?alt=media&token=7cd87887-93d4-4c41-8952-db82777e1117)

{{[[table]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FbMLzO7q-5M.png?alt=media&token=d3fb0597-9eab-4c3d-a9f0-8ff72ab2f086)


After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FItNe6Dk54D.png?alt=media&token=116c8d07-837a-43f6-9020-a0e9b23f9fe1)

Updated Sharing settings

{{[[table]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FuWcVSPMzHQ.png?alt=media&token=fd0ca15c-03e6-49c6-91f4-3bc352450dbc)

After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2F6sPn5_q0gs.png?alt=media&token=74e2fa98-7488-4729-b0e8-7b664692aa79)

And with the page sharing security warning:

{{[[table]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2F5JbnowYACh.png?alt=media&token=886f3455-154f-4c9c-b5da-8ce127517675)

After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FkzwI4ilx0f.png?alt=media&token=14985bc9-daaa-474d-91d1-8511632b8dbf)

The sharing options:

{{[[table]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2F1Nz_WX-5rJ.png?alt=media&token=1e9f9b67-22b6-43c2-b244-beee49393e46)

After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FgKV0seo2nF.png?alt=media&token=61a7206b-6dd5-4ccd-b7c3-429e6dff7522)

Lighter Roam bullets, slightly thinner bold text, and subtler multibar so you can focus on your content

{{[[table]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2F6mUQuhMfeY.png?alt=media&token=3e46c965-ad22-45a5-ba51-4fce71a60283)

After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FOWqQH4AWhh.png?alt=media&token=c19e6e1e-ca64-4a30-b4c3-35b0e4177deb)

[[April 6th, 2021]]

### [[Quality of Life Improvements]] ✨

1. **Kanbans are now directly editable**

Navigate around with key commands (cmd-<arrow> on Mac)

Relocate cards with key commands (cmd-shift-<arrow> on Mac)

Reorder with drag n' drop

Drag and drop blocks in and out of the kanban with more precise location control

Edit cards in the kanban

Enter adds a card below and focuses it

Click in a column to add a card

### [[Bug Fixes]] 🛠

Minor performance improvements

[[April 5th, 2021]]

### [[Bug Fixes]] 🛠

Fixed a memory leak and improved performance

[[April 2nd, 2021]]

### [[Quality of Life Improvements]] ✨

Added shortcut hint in context menu for copying [[Block References]]

Made it clearer that deleting a graph doesn't immediately allow using its name again

{{[[table]]}}

Before::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2F5j3PFaZ5Xz.png?alt=media&token=6d36fc43-b6bc-434d-98fa-22250b6416c9)

After::

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam-team%2FkDgsAI3wOK.png?alt=media&token=07e6f288-00dd-4a03-ac21-1d10ea038f3d)

### [[Bug Fixes]] 🛠

Update Changelog link in `Check for Updates` toast

[[March 30th, 2021]]

### [[New Features]] 🚀

1. You can now export the block you're zoomed into instead of the whole page

### [[Quality of Life Improvements]] ✨

1. Block embeds are now resolved to text in [[Markdown]] exports
2. Added an icon to easily access the right sidebar
The shorcuts icon has been turned into an option inside the ... dropdown menu

3. Added better visual feedback for adding/removing shortcuts

### [[Bug Fixes]] 🛠

Strikethrough and redo shortcuts on Windows have been reverted to Win+Y and Ctrl+Y respectively following reports that users couldn't redo more than once.

[[March 28th, 2021]]

### [[New Features]] 🚀

You can now export in [[Flattened Markdown]], which removes all indentation and block formatting

### [[Quality of Life Improvements]] ✨

1. [[Block Embed]]s will remember whether you closed or opened them between page reloads
2. When editing a page title, any preceding/trailing whitespaces will be automatically removed
3. When exporting a single [page]([[Pages]]), you'll directly receive the exported file instead of a zipped file.

[[March 24th, 2021]]

### [[New Features]] 🚀 

New Help Graph!

### [[Quality of Life Improvements]] ✨ 

Added warning banner to experimental graphs 

[[roam/comments]]

[[February 2nd, 2022]]

[[Joshua Brown]]

Unlimited graphs for all

* not for beta users

