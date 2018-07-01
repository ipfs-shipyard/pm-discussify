# Design workflow

In order to keep the project organised, and so that everyone understands where and how to find the material, here's a detailed description of the folder structure to support the design workflow.

## Folder structure

Folders roughly represent different development stages:

- `input`: Everything you use as input for the project, like inspiration, community feedback and other notes. This can contain files, documents, notes, etc.
- `assets`: Photos, vectors, icons and other design elements you use to put together the designs. In other words, everything that is a part of your final layout should go here.
- `design`: Where you keep the actual design files, the stuff you work on. Typically, it should contain nothing else but a list of files with the designs in various versions or revision stages. Remember, all files used to construct those designs, like photos or icons, should go into the `assets` folder.
- `production`: All final files for delivery to the development team. For print projects, this is where you place your prepress files which can be sent to the printer, like PDF’s fonts and so on. For web projects, this is where you put the mockups with specs, or actual HTML version of the site, if you do the coding too.

So where will you find the photo you’ve been using in the Halloween poster project? In the `assets` folder. How about a file ready for printing? In the `production` folder.

### Versioning

Poor versioning typically looks like this:

- `Brochure Final.png`
- `Brochure Final - image fix.png`
- `Brochure Final Final.png`
- `Brochure Final of all finals – cover page fix.png`
- `Brochure Final Final Final.png`
- `Brochure Final Final Final What Am I Doing.png`

Considering the word `final` is very subjective and impractical, always use numeric versioning:

- `brochure_a_1.png`
- `brochure_a_2.png`
- `brochure_a_3.png`
- `brochure_b_1.png` (note that since this is actually alternative `b`, the version starts from 1)
- `brochure_b_2.png`

What happens if down the road, and let's say you're in version `17`, and you absolutely want to go back to version `9` and continue from there? Just copy version `9` into a version `18` and carry on from there.

If you're confused on what `a` and `b` mean, they are different approaches to the same brochure. Do not get it confused with versions. A version, is another iteration on the same concept, while an `approach` is a different concept. If you're doing an halloween brochure, you might try two different concepts, one around pumpkins and another around witches, and each will have different versions while you iterate on them. This would translate into having files like `brochure_pumpkins_1.png`, `brochure_pumpkins_2.png`, `brochure_pumpkins_3.png`, and so on, and `brochure_witches_1.png`, `brochure_witches_2.png`, `brochure_witches_3.png` and so on.

### Organising filling folders

Projects are typically composed of several subjects/sections, which then need to be organised. In order to avoid scalability issues, these folders follow a few conventions.

#### Generic conventions

- **Allowed characters**: Whenever naming something, unless instructed otherwise, always use lowercase alpha-numeric characters and hyphens, **NEVER** spaces and underscores. Reference regex: `[a-z0-9][a-z0-9\-]*`
- **Subject folders:** If you need to group multiple subjects or sections that heavily relate to each other, name the sections and create folders for each. For instance, you could have the folders `artist-profile`, `library` and `account` inside the `design` folder, each representing different areas of the project.


#### `input` conventions

- **Community input:** Everything the community provides as input for the project goes into a `community` folder.
- **Inspiration:** Everything you use as inspiration for the project goes into `inspiration`

#### `assets` conventions

- **Versioning:** Always version your assets. If you need to store a `banner.png`, store it as `banner_1.png`.
- **Updating:** Do not update assets. Let's say you need to update the `banner_1.png` file. Instead of replacing it, create a `banner_2.png` file and use that. This guarantees that any design pointing to that `banner_1.png` will still work as expected.

#### `design` conventions

- **File naming:** Files inside these *section folders* follow the pattern `[purpose]_[alternative]_[version].[extension]`. Taking the `design/artist-profile` folder as an example, you could have a file named `overview_a_13.png`. Here's a breakdown of what this means:
    - `purpose: overview`: Sections typically have multiple purposes (possibly states). This file represents the `overview` purpose. You could have something like `feed`, `videos`, `discography` here.
    - `alternative: a`: You might need to create several approaches before deciding which one to take. This is where you can name that alternative. Avoid using colour names or anything else that you might want to change meanwhile and render the name useless. It's actually less confusing if you just name it alternative `a`, `b`, `c`, or instead name it with something semantically relevant for the reason of that approach, like `minimalistic` or `cartoonish`. Remember to **always** use an alternative identifier, because you never know when you'll be creating an alternative.
    - `version: 13`: The version number of the file. More on versioning below.
    - `extension: png`: The extension of the file.

#### `production` conventions

- **Consistent naming:** Avoid using versioning when exporting to production. Files should be clearly named after what they accomplish, not their version. So, if you have `artist-profile_a_34.psd` in your designs, you should probably export it as `artist-profile.png`, and always overwrite when creating new versions.
- **Subject folders:** When possible, try to follow the same organisation you have on the `design` folder.

## Example

Here's a simplified, hypothetical organisation:

```
- input
    - briefing.md
    - community
      - user-survey-20180629.xls
    - inspiration
      - foo.jpg
- assets
    - logo
    - backgrounds
    - team-pictures
    - icons
- design
    - desktop
      - account
      - artist-profile
      - library
    - mobile
      - account
      - artist-profile
      - library
- production
  - desktop
    - account
    - artist-profile
    - library
  - mobile
    - account
    - artist-profile
    - library
```

---

This document is based on [How to keep your design files neat and tidy](http://99designs.com/designer-blog/2013/02/06/how-to-keep-your-design-files-neat-and-tidy/).
