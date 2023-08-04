# Utility USS

[Tailwind CSS](https://tailwindcss.com) style utility classes for Unity stylesheets.

## Differences from Tailwind CSS

1. No half sizes (example: `mt-0.5`, `px-3.5`).
2. Fractions in classes converted to words (example: `h-1/3` => `h-one-third`)
3. `font-bold` and `font-italic` combined into `font-bold-italic`

## Usage

Copy `dist/Utility.uss` over to your Unity project and include it in your UXML document.

### Example

```xml
<ui:UXML xmlns:ui="UnityEngine.UIElements" xmlns:uie="UnityEditor.UIElements" xsi="http://www.w3.org/2001/XMLSchema-instance" engine="UnityEngine.UIElements" editor="UnityEditor.UIElements" noNamespaceSchemaLocation="../../UIElementsSchema/UIElements.xsd" editor-extension-mode="False">
  <Style src="project://database/Assets/Utility.uss" />

  <ui:VisualElement class="w-full h-full bg-slate-300 items-center jusitfy-center">
    <ui:VisualElement class="w-48 p-12 text-center">
        <ui:Label text="Hello world!" class="text-slate-900 text-2xl">
    </ui:VisualElement>
  </ui:VisualElement>
</ui:UXML>
```

## Development

First make sure you have nodejs installed on your system. Then run:

```
npm install
```

If you're actively developing run:

```
npm run dev
```

To create a production ready build run

```
npm run build
```

## Not implemented

The following uss properties have not been implemented:

```
-unity-slice-bottom
-unity-slice-left
-unity-slice-right
-unity-slice-scale
-unity-slice-top
```

## Notes

I'm in no way affiliated with [Tailwind CSS](https://tailwindcss.com). I just like Tailwind CSS on web projects and wanted something similar I could bring to Unity.
