# Modulation: how to look after the site

For Admin, and for anyone who looks after the site later. You do not need to know any code.

## The two addresses

- **The site:** https://artsciencemodulation.github.io/Modulation/
- **The editor:** https://artsciencemodulation.github.io/Modulation/admin/

The editor is a set of forms. You change something, press Publish, and the site updates by itself.

---

## Every time you edit (the same five steps)

1. Open the **editor** address and click **Login**. Use the email you were invited with.
2. On the left, click **Site**. Pick the section you want (the list is below).
3. Change what you need. Add or remove things with the buttons in the form.
4. At the top, click **Publish**, then **Publish now**.
5. Wait one to two minutes, then reload the site. If you still see the old version, hold **Ctrl + Shift + R** (on a phone, close the tab and open it again).

**Tip:** make all your changes first, then publish once. Every Publish rebuilds the site, so ten small publishes in a row are slower than one.

---

## What each section is

| Section in the editor | What it controls |
|---|---|
| Settings, theme & menu | Site name, the banner along the top, light or dark background, the accent colour, heading font, menu names, which menu tabs are shown, the footer |
| Home page | Opening text, the felt ↔ measured dial, the quotation, the film |
| The exhibition (panels) | The six panels: text, artworks, science images, colour viewers, info cards |
| Take part (body map) | The body-map page and its words |
| Make a mark (drawing page) | The online drawing page |
| Invited artists | One room and one menu tab for each invited artist |
| Workshops | Each workshop, its poster and photos |
| Lineage | The art links, the science links and the essay |
| Contributors | The people, their roles and short bios |
| Extra pages (add a new tab) | Brand-new pages, built from blocks |

---

## Common jobs

**Change some text.** Open the section, click in the box, type, then Publish.

**Replace a picture.** Click **Choose different image** under the picture and upload the new one. Then Publish. Read "Picture rules" below first.

**Add a new felt ↔ measured pair.** Home page → "Felt ↔ measured pairs" → **Add**. Fill in the artwork, the science image, a short description of each (this is read aloud for people who can't see the image), the captions and the credit. If the artwork looks too big on the dial, lower the **Felt size** (1 is normal, 0.8 is smaller with a thicker border).

**Remove something.** Each item in a list has a small **×** (delete) button at the top of the item. Click it, then Publish.

**Change the order.** Drag the **≡** handle on an item up or down.

**Put in the new video.** Home page → **Film**. Paste the YouTube video's code (the letters after `v=` in its address), tick **Show the film**, then Publish. Untick it to hide the film again.

**Add an image to an exhibition panel.** The exhibition (panels) → the panel → **Images** → Add. Choose honestly under *What kind of image is this?*: **Artwork**, **Science image**, or **Art made on a science image**. A micrograph the artist has drawn on is the third kind, never the second.

**Add a science link.** Lineage → **Science links** → Add. Give it a title, where it is from, one line on what it is, the link text and the address.

**Add a person to Contributors.** Contributors → **People** → Add. Name, role, short bio.

**Hide or show a menu tab.** Settings, theme & menu → the menu part → switch the tab on or off.

---

## Now and then

**Add an invited artist.** Invited artists → **Add artists**. Give a name, a menu name, a one-word web address (for example `manika`, small letters only) and tick *Show in menu*. Then add **Sections**: each is either a *Row of images* or a *Book with magnifying lens* (like the Diary Pages). When work is still to come, tick *Work still to come*; untick it when the work arrives.

**Add a new page (a new menu tab).** Extra pages → **Add pages**. Give a title, a menu name and a one-word web address. Then build the page from blocks. You can use: Text, Heading, Image, Gallery, Quotation, Prompt, Links and Video (YouTube). Add as many blocks as you like and drag them into order.

**Add a workshop.** Workshops → add a new entry with its poster, description and prompts. Only add photos of participants' work if they agreed to have it published. Fill in *Made by* only if the maker asked to be named.

**Add a colour viewer ("Colour is a choice").** The exhibition (panels) → the panel → **Colour-map viewers** → Add. Upload the same image in each colour version, and keep all versions the same size.

**Change how the whole site looks.** Settings, theme & menu → **Theme**. You can choose a dark or light background, pick the accent colour, and pick the heading font from a short list. None of these can break the site.

---

## Picture rules

- Keep each picture **under about 1 MB** and about **1500 pixels** on the long side. Photos straight from a phone are too big.
- To shrink one for free, open **squoosh.app** in your browser, drop the picture in, set the width to 1500 and download it. A JPEG or WebP file is fine.
- If an upload fails, the picture is almost always too big.
- Give every image a short description in the "description" box. It is what screen readers say aloud.

---

## Rules of this site

- The paintings try to catch the experience of pain. They are not science illustrations. Keep art and science side by side, each labelled for what it is.
- Only publish work by participants, or lab images, when you have permission.
- Nothing here is medical advice or a way to test yourself. Keep wording to "describing", not "diagnosing".
- Link to museums and papers. Do not copy their pictures onto the site.

---

## Who can do what

**Editors** (like you) change content. They only need an email address. They do not need a GitHub account.
- To add an editor, the owner invites their email in DecapBridge (the login service). There can be up to ten editors at a time.

**Owners** look after the accounts behind the site. The site lives in a GitHub organisation called `artsciencemodulation`. There should always be **two owners**, so that nobody is locked out.

Once a year, the owner has to renew the access key that lets the editor save changes (it is called a *token* and expires). 
IMPORTANT: Renewal date: "November 27, 2027"

---

## If something goes wrong

| What you see | What to do |
|---|---|
| The site hasn't changed after publishing | Wait two minutes. Reload with Ctrl + Shift + R. Check you clicked *Publish now*. |
| The editor won't let you log in | Look for the invitation email and check spam. Otherwise ask an owner to invite you again. |
| A picture won't upload | Make it smaller (see Picture rules). |
| You published something by mistake | Tell an owner. Every change is saved and can be undone. |
| A page looks broken or blank | Stop editing and tell an owner what you changed last. |

---

## What needs a developer

Everything above can be done without code. You need a developer only for a brand-new *kind* of interactive piece (something that behaves unlike the dial, the body map, the magnifying lens or the colour viewer), or for a full redesign. After it is built once, its content is editable here like the rest.
