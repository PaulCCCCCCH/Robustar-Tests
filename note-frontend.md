# Frontend Testing

Cypress best practice:

https://docs.cypress.io/guides/references/best-practices



## Tags for Testing

Add `data-test` attribute to an HTML tag if it is hard to select with selector.

For example, in `ImageList`, add a tag to image:

```html
<div v-for="(url, idx)" in imageList">
   <v-img ... :data-test="`image-list-img-${idx}`">                          
</div>

```

Then the first image DOM can be selected with

```javascript
cy.getBySel("image-list-img-1")
```

**Important**:
- Naming of the `data-test` attribute should be `<component-name>-<dom-element-name>-<name>`, for example, `image-list-input-page-number`.
- Try not to use `cy.contains` and search for things like button names, otherwise test cases won't work when text is changed in the future versions.


## Reusability

Many manipulations are shared across tests for multiple components and can be modularized for reuse. For example, "open image, edit, send edit, then go back" will be used to test image editor, image list on annotated split, paired training, etc.

To allow reuse, create commands in `front-end/cypress/support/commands.js`.

More on custom command:

https://docs.cypress.io/api/cypress-api/custom-commands#Overwrite-Existing-Commands





## More to be added...