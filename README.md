# personal-landing-page

Simple landing page similar to linktr.ee  
Includes a dark mode with automatic detection

### Installation

- Fork this repository

### Customization

- `/src/components/Headline.astro` is the site headline
- `/src/components/Blurb.astro` is your bio/welcome text
- `/site.config.js` contains your site title and link collection.

  Your site content is an array of objects:

  ```
  [{
    headline: "My websites",
    links: [
      {
        title: "zaps.lol",
        href: "https://zaps.lol",
        icon: "/pages/zaps-lol.png",
        // emoji: '⚡',
        body: "Free nostr address provider",
      }, …
    ]
  }, …]
  ```

  Every link can have these properties:

  - `title`: Link title
  - `href`: Link URL
  - `icon`: Link icon - add your icon to `/public` and add icon path as `/`.  
    Example: Image path is `/public/github.svg` - `icon` property is `/github.svg`
  - `emoji`: String of an emoji which will be displayed as icon.  
    Copy e.g. from [emojipedia](https://emojipedia.org).  
    You should use either an icon or an emoji, not both!
  - `body`: Short descriptive text

### Deployment

This project deploys to Github pages by default.  
Just enable it in the repository settings.

Edit `CNAME` to fit your domain name if you want to use one.

---

Built with [Astro](https://astro.build)
