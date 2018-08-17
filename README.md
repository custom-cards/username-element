# Username Element

This element is **not** all that useful as a card (it can be used for that to), the purpose of this is to give the option to add static text on a `picture-elements` card.

## Options

| Name | Type | Default | Description
| ---- | ---- | ------- | -----------
| type | string | **Required** | `custom:username-element`

## Installation

### Step 1

Install `username-element` by copying `username-element.js`from this repo to `<config directory>/www/username-element.js` on your Home Assistant instanse.

**Example:**

```bash
wget https://raw.githubusercontent.com/custom-cards/username-element/master/username-element.js
mv username-element.js /config/www/
```

### Step 2

Link `username-element` inside you `ui-lovelace.yaml`.

```yaml
resources:
  - url: /local/username-element.js?v=0
    type: js
```

### Step 3

Add a custom element in your `ui-lovelace.yaml`

```yaml
      - type: picture-elements
        image: /local/files/LUfuf8ow.jpg
        elements:
          - type: custom:username-element
            style:
              top: 59.6%
              left: 26.8%
```