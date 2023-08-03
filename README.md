# Utility USS

[TailwindCSS](https://tailwindcss.com) style utility classes for Unity stylesheets.

## Differences from Tailwind CSS

1. No half sizes (example: mt-0.5, px-3.5).
2. Fractions in classes converted to words (example: h-1/3 => h-one-third)

## Usage

Copy `dist/utility.uss` over to your Unity project and include it in your UXML document.

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

## Todo

The following uss properties still need to be implemented:

```
rotate
scale
transform-origin
translate
-unity-background-image-tint-color
-unity-background-scale-mode
-unity-font-definition
-unity-overflow-clip-box
-unity-paragraph-spacing
-unity-slice-bottom
-unity-slice-left
-unity-slice-right
-unity-slice-scale
-unity-slice-top
-unity-text-outline
-unity-text-outline-color
-unity-text-outline-width
-unity-text-overflow-position
```

## Notes

I'm in no way affiliated with [Tailwind CSS](https://tailwindcss.com). I just like Tailwind CSS on web projects and wanted something similar I could bring to Unity.
