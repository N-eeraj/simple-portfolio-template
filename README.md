# Portfolio Template

### Getting Started
- Fork the repository
- Install dependencies
  `npm i`
- Setting Base URL
  Currently the base URL will be `/` for dev build & `/simple-portfolio-template/` for the production build.
  This can be changed accordingly, and if you don't any base URL in neither dev or production builds, just remove the following lines from the `nuxt.config.ts` file.
  ```
    app: {
      baseURL: process.env.NODE_ENV === 'production' ? '/simple-portfolio-template/' : '/'
    },
  ```
- To start the development server
  `npm run dev`
- To build the production files
  `npm run generate`

### Tech Used
- [Nuxt](https://nuxt.com/)
- [UnoCSS](https://unocss.dev/)
- [Nuxt Google Fonts](https://google-fonts.nuxtjs.org/)
- [Animate on Scroll](https://nuxt.com/modules/aos)
- [Nuxt Image](https://image.nuxt.com/)
- [Nuxt Icon](https://nuxt.com/modules/icon)

#### Data   
Portfolio data is taken from the files present in the `data` directory, replace them with the desired content.
The files are to be put in the `public` directory if a local image is needed to be used, a relative path is to be used in the data files. If an online image is needed to be used, just use the image URL in the data files.
The icons has to be a valid iconify icon, you can browse them [here](https://icon-sets.iconify.design/).

### Theming
The UI colors are taken from the `color.json` file in the `theme` directory, it can be changed as desired.
- `primary` is the background color of the page.
- `secondary` is the color of the text, links & buttons etc.
- `accent` color is used for certain indication.

Make sure the primary contrasts with the secondary when switching up the theme.

> Design inspiration from [Magic UI](https://magicui.design/docs/templates/portfolio)

### Features/Sections

- Hero
- About
- Skills
- Experience
- Footer
