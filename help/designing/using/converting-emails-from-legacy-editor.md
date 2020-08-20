---
title: Converting Legacy Editor Email to the Email Designer 
description: Discover how to use emails created in the Legacy Editor Email to the Email Designer.
page-status-flag: never-activated
uuid: 571ffc01-6e41-4501-9094-2f812b041a10
contentOwner: sauviat
products: SG_CAMPAIGN/STANDARD
audience: designing
content-type: reference
topic-tags: editing-email-content
discoiquuid: 39b86fda-7766-4e5f-ab48-bcc536ab66b3

internal: n
snippet: y
---

# Converting Legacy editor email content {#converting-an-html-content}

Start working with the Email Designer and build reusable templates and fragments from your email HTML created in the Legacy Editor.

This use case enables you to create an Email Designer template by using an HTML email and dividing it into HTML components in the Email Designer. 

>[!NOTE]
>
>Like the compatibility mode, an HTML component is editable with limited options: you can only perform in-place edition.

>[!IMPORTANT]
>
>This section is for advanced users who are familiar with HTML code.

## Preparing your email content

1. Select an HTML email. 
1. Identify sections to divide the HTML email.
1. Cut out the different blocks from your HTML. 

## Create your email structure 

1. Open the **[!UICONTROL Email Designer]**  to create an empty email content.
1. Set the body level attributes: background colors, width, etc. For more on this, see [Editing email styles](../../designing/using/styles.md).
1. Add as many structure components as you have sections. For more on this, see [Editing the email structure](../../designing/using/designing-from-scratch.md#defining-the-email-structure).

## Add HTML content

1. Add an HTML component to each structure component. For more on this, see [Adding fragments and components](../../designing/using/designing-from-scratch.md#defining-the-email-structure).
1. Copy-paste your HTML into every component.

## Manage the style of your email {#manage-the-style-of-your-email}

1. Switch to **[!UICONTROL Mobile view]**. For more on this, see [this section](../../designing/using/plain-text-html-modes.md#switching-to-mobile-view).

1. To fix this, switch to source code mode and copy-paste your style section into a new style section. For example:

   ```
   <style type="text/css">
   a {text-decoration:none;}
   body {min-width:100% !important; margin:0 auto !important; padding:0 !important;}
   img {line-height:100%; text-decoration:none; -ms-interpolation-mode:bicubic;}
   ...
   </style>
   ```

   >[!NOTE]
   >
   >Make sure you add your style after this in another custom style tag.
   >
   >Do not modify the CSS generated by the Email Designer:
   >
   >* `<style data-name="default" type="text/css">(##)</style>`
   >* `<style data-name="supportIOS10" type="text/css">(##)</style>`
   >* `<style data-name="mediaIOS8" type="text/css">(##)</style>`
   >* `<style data-name="media-default-max-width-500px" type="text/css">(##)</style>`
   >* `<style data-name="media-default--webkit-min-device-pixel-ratio-0" type="text/css">(##)</style>`

1. Go back to the mobile view to check that your content is correctly displayed and save your changes.

## Use Case

Let's try to convert this email, created in the legacy editor, into an **[!UICONTROL Email Designer]** template.

## Identify the section of your email 

We can identify 11 sections in this email. 

![](assets/html-dce-view-mail.png)

To identify which element is which section of the HTML, you can select it.

![](assets/breadcrumbs.png)

To see the HTML version of the email, click **[!UICONTROL Show source]**.

### Create the email template and its structure 

1. Drag and drop **[!UICONTROL Structure components]**  reflecting the layout of our email. 

1. Repeat as many times as needed. We need to create 11 structure components.

   ![](assets/structure-components-migration.png)

### Inserting HTML content components

1. Insert an **[!UICONTROL HTML component]**  in each **[!UICONTROL Structure component]** .

   ![](assets/html-components.png)

1. For each section, click **[!UICONTROL Show source code]** .

   ![](assets/show-source-code.png)

1. Insert the HTML section.

1. Click **[!UICONTROL Save]**.

You can now check the rendering of your email.

![](assets/migrated-email-result.png)

### Managing styles to fit mobile view

1. Insert CSS elements to ensure that your email is suitable for mobile view.

1. Switch to source code and copy-paste your style section into a new style section.

For more on this, refer to [Manage the style of your email](#manage-the-style-of-your-email).

Your legacy email is now available in the Email Designer. 