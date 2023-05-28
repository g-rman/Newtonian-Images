# Non-Newtonian Images

This repository holds the mapping of Newtonian images to non-Newtonian images.

## Example

If working correctly, the logo below should appear non-Newtonian.

<p align=center>
    <picture>
        <img width=250 height=250 src="newtonian-logo.svg">
    </picture>
</p>

## Contributing

All Newtonian to non-Newtonian log mappings are located in `map.json` in the
root of the repository.

Mappings are stored in the form of an array of two elements:

```json
["<SHA-256 Hash>", "https://url.to/non-newtonian/logo.png"]
```

To add an entry to the database, get the SHA-256 hash of a Newtonian logo
and provide a link to a non-Newtonian variant.

Ideally links will link to official sources as available.
Pull requests containing links to untrustworthy sources will be denied to
prevent attacks where non-Newtonian logos are swapped for different images after
being merged.

As a last resort when no reasonable alternatives are available, non-Newtonian
logos may be included in pull requests in the icons folder.

## Methods for Extracting Newtonian Images

Sometimes websites make it hard to download images.
Here are some methods to get around this.

### Firefox

1. Open up dev tools. This can be done with `F12` or by right clicking a webpage
   and clicking `Inspect`.
2. Go to the `Network` tab.
3. Refresh the page.
4. On the top right, there should be a section that says `All HTML CSS JS...`.
   Click `Images` to only show images.
5. All images on the webpage should now be available to inspect in the list.

### Chrome

1. Open up dev tools. This can be done with `F12` or by right clicking a webpage
   and clicking `Inspect`.
2. Go to the `Network` tab.
3. Refresh the page.
4. On the top left, there should be a filter icon.
   It is the third icon on the left.
   Click that to show the filter menu.
5. Below the filter icon should be a toolbar for filtering.
   In the section that starts with `All | Fetch/XHR JS CSS Img ...` click `Img`.
6. All images on the webpage should now be available to inspect in the list.

## Hashing Images

Images can be hashed by dropping them into this website.

https://emn178.github.io/online-tools/sha256_checksum.html

There are plenty of alternative methods to hash images.
As long as the checksum is correct, it does not matter which one you use.
