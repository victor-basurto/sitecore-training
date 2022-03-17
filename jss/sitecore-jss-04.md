## Mock Data
**Mocking Data**
- When to Mock data
Mock Data by copying files, image fields, and other items into the file system.

- Reuse Content
    Reuse content when you need to use the same content in multiple locations such as `Headers` and `Footers` can be reused across multiple pages.

- Work Disconnected
    Work disconnected from **Sitecore** to create components and mock route data.
    - When the app runs, it does not have the data from **Sitecore** using `HTTP` data calls.
    - You're using a local `datasource` for your content, route (layout), and component registrations.

#### Using Styleguide data Types

**Route-Level Fields Data**
- To Mock `route-level` fields. simply add a `fields` property to your route data.
```json
{
  "name": "route",
  "template": "MyRoute",
  "displayName": "Route",
  "fields": {
    "metaTitle": "My Route",
    "titleText": "My Route",
    "body": "Lorem ipsum dolor sit"
  },
  "placeholders": {
      // ...
  }
```

**Image Field**
Example of how to use the `<img>` field in `vue`
```html
Plain image
<sc-image :media="fields.sample1" />

Advanced image (not editable)
<sc-image
  :media="fields.sample2"
  :editable="false"
  :imageParams="{ mw: 100, mh: 50 }"
  height="50"
  width="94"
  data-sample="other-attributes-pass-through"
/>

Srcset responsive image
<sc-image
  :media="fields.sample2"
  :srcSet="[{ mw: 300 }, { mw: 100 }]"
  sizes="(min-width: 960px) 300px, 100px"
  class="img-fluid"
/>
```
```html
<script>
  import { Image } from '@sitecore-jss/sitecore-jss-vue';
  import StyleguideSpecimen from './Styleguide-Specimen';

  export default {
    name: 'Styleguide-FieldUsage-Image',
    props: {
      fields: {
        type: Object,
      },
      rendering: {
        type: Object,
      },
    },
    components: {
      ScImage: Image,
      StyleguideSpecimen,
    },
  };
</script>
```
1- _How Route Provides Mock Data:_
The data is acquired from the local `datasource` and runs on a local development server.

2- _Using Styleguide Data Types:_
Helps mock data.

3- Route-Level Fields Data: 
Mocks route-level fields by simply adding `fields` property to your route data.
