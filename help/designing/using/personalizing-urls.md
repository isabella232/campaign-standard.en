---
title: Personalizing URLs
seo-title: Personalizing URLs
description: Personalizing URLs
seo-description: Learn how to personalize URLs in a delivery by adding personalization fields, content blocks, or dynamic content.
uuid: 686a44d2-9602-44e3-a902-82daaff2de01
content-encoding: ISO-8859-1
aemsrcnodepath: /content/help/en/campaign/standard/designing/using/personalizing-urls
contentOwner: sauviat
cq-designpath: /etc/designs/help
cq-lastmodified: 2018-09-10T07 26 12.903-0400
cq-lastreplicated: 2018-09-07T15 07 41.182-0400
cq-lastreplicatedby: sauviat
cq-lastreplicationaction: Activate
products: SG_CAMPAIGN/STANDARD
audience: designing
content-type: reference
topic-tags: managing-links
cq-template: /apps/help/templates/article-3
discoiquuid: 79779d58-f558-461f-aa3a-9be28be13aea
firstPublishExternalDate: 2018-09-07T15:07:40.611-0400
herogradient: light
isreadyforlocalization: false
jcr-created: 2018-03-15T09 02 17.185-0400
jcr-createdby: admin
jcr-description: Personalizing URLs
jcr-ischeckedout: true
jcr-language: en_us
lastPublishExternalDate: 2018-09-07T15:07:40.611-0400
lochandoffdate: 2018-09-10T07 26 12.902-0400
loclangtag: locales fr;locales de;locales ja
lr-lastreplicatedby: sauviat@adobe.com
navTitle: Personalizing URLs
publishexternaldate: 2018-09-07T15 07 40.611-0400
publishExternalURL: https://helpx.adobe.com/campaign/standard/designing/using/personalizing-urls.html
sha1: ef1d4400b06adedc4810b09a62b278f6fda1a5c3
topicBrowsingSortDate: 2018-09-07T15:07:40.611-0400
index: y
internal: n
snippet: y
---

# Personalizing URLs

Personalizing URLs

Adobe Campaign allows you to personalize one or several URLs in your delivery by adding personalization fields, content blocks, or dynamic content to them. To do this:

* Insert an external URL and specify its parameters. See [Inserting a link](../../designing/using/inserting-a-link.md).
* If not displayed, click the pencil next to the selected URL in the side pane to access the personalization options.
* Add the personalization fields, content blocks, and dynamic contents that you want to use.

  ![](assets/des_personalize_links.png)

* Confirm your changes.

>[!NOTE]
>
>Personalizing URLs cannot be applied to the domain name, nor to the URL extension. An error message will be displayed during delivery analysis if personalization is incorrect. When selecting a content block, you are not allowed to select elements such as **Link to mirror page**. This type of blocks is forbidden inside a link.

To change a personalized URL, select it and use the **URL** button in the palette on the left-hand side.

In the [content editor](../../designing/using/about-email-content-design.md#using-the-email-content-editor), the **Encoded value** option is checked by default. It allows for special characters to be encoded if they are present in the personalization field's value. We advise you to leave this option unchecked to avoid incorrect URL encoding.

![](assets/delivery_content_59.png)

**Related topics**:

* [Inserting a personalization field](../../designing/using/inserting-a-personalization-field.md)
* [Adding content blocks](../../designing/using/adding-a-content-block.md)
* [Defining dynamic content](../../designing/using/defining-dynamic-content-in-an-email.md)
