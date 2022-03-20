# Metagros
![](https://github.com/igsr5/metagros/workflows/CI/badge.svg)
![](https://img.shields.io/badge/license-MIT-green)

Metagros is a tool to get OGP data from the site URL.


![](https://static.wikia.nocookie.net/pokemon-radiance/images/0/01/059_Metagross.png/revision/latest/scale-to-width-down/308?cb=20200304023123)  
https://pokemon-incandescent.fandom.com/wiki/Metagross

## Features
- Node.js ESM module
- Get `og:OOO` content data from site url
  - e.g.  `<meta property="og:title" content="metagros page" />` → get `"metagros page"`
- Less dependenceies
- Popular Pokémon
  - so cool!! cute!! intelligence!!!


## Installing
Using npm
```sh
$ npm install metagros
```
Using yarn
```sh
$ yarn add metagros
```

## Example

🚧 wip...

main.js
```ts
import { getPageMetaData } from "metagros";

const url = "https://some.com";

const metadata = await getPageMetaData(url);
console.log(metadata);
```

```ts
$ node --experimental-specifier-resolution=node ./main.js
{
  title: "Site title",
  description: "Site description.This site is OO's HP ...",
  image: "https://images.com/hoge",
  type: "article",
  siteName: undefined,
  url: "https://some.com"
}
```



## License
See [LISENSE](https://github.com/igsr5/metagros/blob/master/LICENSE).
