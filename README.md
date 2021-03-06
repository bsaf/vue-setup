# Vue setup checklist

Prototyping setup for new Vue projects.

**Vue plugins**

- [ ] Use Vue Router
- [ ] Use Vuex

**Project setup**
- [ ] Create a `components` and `views` folder
- [ ] Put a [BlankComponent.vue](BlankComponent.vue) template in `/components`

**Styling and assets**
- [ ] Add [Basscss](http://basscss.com/) (see below), or try [Tachyons](http://tachyons.io/docs/)
- [ ] Put fonts, images, sass into a single `assets` folder
- [ ] Set up colours in `variables.scss`
- [ ] Import your [own toolkit additions](basil-toolkit.scss) as a single CSS file
- [ ] Create a single CSS file for project-specific toolkit styles
- [ ] Override h0-h6 in the file above with project-specific type
- [ ] Import the CSS files in main.js
- [ ] Import and set up fonts

**Other plugins**
- [ ] Add Element UI (see below)

<hr/>

### CSS additions

```
$ yarn add basscss

// in main.js
import 'basscss/css/basscss.css'
import '../assets/sass/global'
import '../assets/sass/basil-toolkit'
```

### Adding Element UI

Check the [documentation](http://element.eleme.io/) for latest install instructions.

```
$ npm i element-ui@next -S

// in main.js
import ElementUI from 'element-ui'
import 'element-ui/lib/theme-chalk/index.css'
Vue.use(ElementUI)
```
